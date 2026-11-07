# Field Camera Lab

A fictional camera explainer with an original SVG elevation. Open `index.html` in a current browser. The app runs offline and uses no dependencies.

- Inspect the lens, viewfinder, or grip to read about the selected component.
- Adjust the aperture to see the iris change and compare relative light to f/2. The simplified model uses the square of the ratio of the two f-numbers.

Ridgeline Optical and Sable 04 are fictional names for this project. The illustrations, text, and software were created independently. [Concept reference](https://github.com/YildizDikme/3d-camera-landing-page)

## Local server and agent connection

Install Node 22 or newer and Git. From this repository run:

```sh
npm ci
npm start
```

Open the loopback URL printed by the command. The runtime is pinned to a specific revision of [Project Agent Bridge](https://github.com/Mert-Oezdemir/project-agent-bridge).

To connect an MCP-compatible agent, run `npm run mcp:config --silent` and add its `mcpServers` entry to your host. Run `npm run doctor` to see local project and account configuration.

Chrome or Edge is needed for agent browser controls. You can set `CHROME` in `.env`, or run `npx playwright install chromium` to install a browser.

Copy `.env.example` to `.env` before adding account settings. Keep `.env` local. Restart the runtime after changing it.
