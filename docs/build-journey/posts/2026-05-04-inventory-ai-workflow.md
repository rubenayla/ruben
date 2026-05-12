# Using an AI Inventory to design PCBs

*Published 2026-05-04 · [Build Journey index](../index.md)*

We're using an AI Inventory to design PCBs.

"Do we have any DAC chips in stock?" If answering that means going on a trip to the workshop and spending an hour looking for them between bags, we're doing something wrong.

![The team photographing components on a tripod rig](../../images/build-journey/2026-05-04-inventory-ai-workflow/01_team_with_tripod.jpg)

Nobody wants to do an inventory, so we made it as easy as possible. We set up a tripod over a workshop table, and took pictures of all 270 bags with components.

![Handwritten LM393P component bag](../../images/build-journey/2026-05-04-inventory-ai-workflow/04_lm393p_handwritten_bag.jpg)

Then, Claude identified each component, looked the manufacturer part number up online for description and datasheet, and saved the data into [Notion](https://www.notion.so/) using their MCP connector. It worked at first try.

![Notion inventory database](../../images/build-journey/2026-05-04-inventory-ai-workflow/03_notion_inventory_database.png)

Now we can ask things like:

> "Hey Claude, we need to generate two analog signals from an ESP32 — one 0–5V, one 0–10V. What can we use from the inventory?"

And get back:

> "Use the DAC7574 (quad 12-bit I²C, 2 in stock). With VREF = 5V, the first channel gives 0–5V directly. For the 0–10V channel, route the second channel through an LM358 wired non-inverting at gain 2 (R1 = R2 = 10 kΩ, both in stock). Power the op-amp from the kart's 12V rail. Heads up: you're down to 2 DAC7574s. Probably worth adding a few to the next Mouser order."

<div style="max-width: 315px; margin: 1em auto;">
  <div style="position: relative; padding-bottom: 177.78%; height: 0;">
    <iframe
      src="https://www.youtube.com/embed/xWUMcP6Wm6w"
      title="Our Inventory is AI — Formula Student kart"
      frameborder="0"
      allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
      style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
  </div>
</div>

Huge thanks to Gabriel Fernández Romero and Adrián for the help.

If you have a similar workflow, try this and share your experience — I'm loving it so far.

---

[:material-arrow-left: Previous: Mounting the motor, and why the first bracket failed](2026-04-29-motor.md){ .md-button }

*That's the latest post. New ones land roughly every Wednesday — [follow on LinkedIn](https://www.linkedin.com/in/rubenayla/) to catch them as they ship, or check back here.*

*[Originally posted on LinkedIn →](https://www.linkedin.com/feed/update/urn:li:activity:7456983051160481793/)*
