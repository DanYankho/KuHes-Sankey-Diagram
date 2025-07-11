📊 Company Learning Department – Growth & Structure Flow (Animated Sankey Diagram)
This project is an interactive and animated Sankey diagram built using D3.js v7 and the D3 Sankey plugin. It visually represents the organizational structure and historical growth flow of a company's Learning Department or related divisions, with a special focus on how teams and sub-units evolved or branched from one another over time.

The visualization allows viewers to understand the lineage and transformation of various teams, highlighting the transition of responsibilities, resource allocation, and the emergence of new departments. Each link in the Sankey chart flows sequentially with custom delays, providing a step-by-step animation of how the structure expanded.

🔍 Key Features
✅ D3 Sankey Layout: Utilizes the d3-sankey layout to compute node positions and link flows.

🎨 Custom Styling: Nodes and links are colored meaningfully to distinguish different stages or units.

⏱️ Animated Transitions: Each link appears with a manual delay, visually narrating the sequence of the department’s growth.

👁️ Progressive Node Reveal: Target nodes fade in as their respective links animate in, guiding the viewer through the flow logically.

♻️ Replay Button: Includes a replay button that restarts the flow animation, useful for demos or presentations.

📱 Responsive Design: Adjusts layout and text for mobile and small screens using media queries.

🧱 How It Works
The data (nodes and links) is defined statically in JavaScript. Each node represents a team/unit and each link represents a connection or evolution from one unit to another.

Every link is assigned a custom delay in milliseconds to control when it appears.

The script loads the data, computes the Sankey layout using D3, and renders nodes and paths.

Each link is drawn progressively using a stroke-dasharray animation to simulate flow.

When a link finishes animating, the target node becomes visible.

The replay button re-invokes the rendering function to play the sequence again.

📂 Folder Structure
plaintext
Copy code
.
├── index.html      # Main HTML file with embedded JS and CSS
├── README.md       # This documentation file
🛠️ Technologies Used
Tool	Purpose
D3.js v7	Visualization library
d3-sankey	Sankey layout plugin
HTML5 & CSS3	Structure and styling
Vanilla JavaScript	Data handling and animation control

📈 Use Case
This tool is ideal for:

Showcasing how a department grew over time

Visualizing internal organizational changes

Presenting reporting structures in presentations or stakeholder meetings

Teaching teams how sub-units interconnect or evolved

✍️ Customization
To modify the flow:

Change the nodes and links in the loadData() function

Adjust the delay values in the links to change animation timing

Customize colors and node padding as needed

🧩 Limitations & TODOs
Nodes are currently placed automatically by D3 with only one manual override (ZBS).

Link values are illustrative; you can use actual metrics (e.g., headcount, budget, etc.) for more insight.

Export to image/pdf is not included yet (could be added using html2canvas or svg-crowbar).

