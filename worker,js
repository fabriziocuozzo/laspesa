const AIRTABLE_TOKEN = "patnaSIB6mZ28y1QZ.075ec69331485aec61caf6863657e4338d0fc69a2bd3e80f4db822a9c92c9aad";
const AIRTABLE_BASE  = "https://api.airtable.com";

const CORS = {
  "Access-Control-Allow-Origin":  "*",
  "Access-Control-Allow-Methods": "GET, POST, PATCH, DELETE, OPTIONS",
  "Access-Control-Allow-Headers": "Content-Type, Authorization",
};

export default {
  async fetch(request) {
    if (request.method === "OPTIONS") {
      return new Response(null, { status: 204, headers: CORS });
    }
    const url  = new URL(request.url);
    const path = url.pathname + url.search;
    const res  = await fetch(AIRTABLE_BASE + path, {
      method:  request.method,
      headers: { "Authorization": `Bearer ${AIRTABLE_TOKEN}`, "Content-Type": "application/json" },
      body:    ["GET","HEAD","DELETE"].includes(request.method) ? undefined : request.body,
    });
    return new Response(await res.text(), {
      status: res.status,
      headers: { "Content-Type": "application/json", ...CORS }
    });
  }
};
