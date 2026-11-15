# Tryon: 360° fit and garment spin

Built at the CV × Google DeepMind hackathon (October 2026).

Tryon works out how a garment will actually fit from your body measurements and the brand's size chart, then shows the result on an interactive 360° turntable.

- **Fit:** compares body measurements with size-chart specs, per measurement, and recommends a size.
- **Turntable:** a three.js 360° viewer for the garment.
- **Compare:** sizes side by side.
- **Gemini:** called server-side from `server.ts`, so the API key never reaches the browser.

## Run it

```bash
cp .env.example .env    # add your Gemini API key
bun install             # or npm install
bun run dev             # serves on http://localhost:3000
```

`bun run lint` type-checks the project.

## Stack

React 19, Vite, Tailwind CSS 4, three.js, Express, `@google/genai`.

## License

MIT
