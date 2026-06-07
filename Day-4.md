---
---

--- Before Day-4 ---

I already knew how to make basic GET and POST requests using `requests` in Python, but I wasn't deeply familiar with analyzing network payloads, HTTP headers, or replicating API calls via the terminal.

---

## Day-4 Checklist

- [x] I know the 5 core HTTP methods (GET, POST, PUT, PATCH, DELETE) and what each is used for
- [x] I can read a status code and know what went wrong – e.g., 401 vs. 403 vs. 404 vs. 500
- [x] I can open Chrome DevTools Network tab, find a request, and inspect its headers, payload, and response
- [x] I can copy a browser request as a cURL command and run it in the terminal
- [x] I can change the `User-Agent` in the browser and see the change in the Network tab
- [x] I can use `curl` to make a GET request with query parameters and a POST request with a JSON body
- [x] I have a running FastAPI app with at least two endpoints (`GET /health` and `POST /echo`)
- [x] I can test my API using the Swagger UI at `/docs` and via `curl` from the terminal

--- After Day-4 ---

I learned these things as well, apart from the checklist:
- How to emulate different mobile devices and change the User-Agent in Chrome DevTools to test UI responsiveness.
- How to parse URL structures to identify domains, paths, and query parameters (e.g., `?client_id=123&force_load=true`).
- How to seamlessly convert network requests from the browser into Python code using the "Copy as cURL (bash)" feature and automated cURL-to-Python converter tools.
- The concept of "Man-in-the-Middle" (MITM) attacks and how tools like Burp Suite can be used to intercept, modify, and spoof requests before they reach the server (like pausing game timers).
---

--- Feedback (Suggestions for the TDS Team) ---

This is my feedback:
The live demonstration of fetching an SVG from the OpenAI API via `curl` and rendering it visually was excellent for bridging the gap between raw data and actual frontend output. I also appreciated the candid advice at the end regarding how non-programmers should approach this diploma—focusing on AI debugging, conceptual semantics, and consistent collaboration on Discourse rather than pure syntax memorization.

---

---
---

You can write your personal notes here; they will not be parsed and are for your own reference.
- DevTools element selection shortcut: `Ctrl+Shift+C`.
- `200 OK` is the golden status code.
- Never commit API keys to GitHub. Use `.env` files and add them to `.gitignore`.
- To emulate slow networks in DevTools, use the "Throttling" dropdown in the Network tab (e.g., "Slow 3G").
- You can pipe API responses into files in the terminal like this: `curl "https://httpbin.org/get" > response.json`.
