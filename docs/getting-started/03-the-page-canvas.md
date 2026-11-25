# The page canvas

A Notus page is not a document that flows top to bottom. It is an **unbounded 2D canvas** — a workbench. Everything you put on a page (text, images, shapes) is a **block** with its own position and size. Blocks can sit anywhere, overlap, and be dragged around freely. There is no required order.

## Create a text block

With the **Select** tool active, **double-click any empty spot** on the canvas. Notus creates a text block there, focused and ready for you to type. Text blocks grow taller automatically as you add lines, so your content stays visible without you resizing them.

A **single** click on empty canvas doesn't make a block — it drops an **insertion point**, a marker showing where pasted content will go. Click once to place it, then paste (Ctrl+V, or Cmd+V on macOS): pasted text becomes a new text block at that spot — and it **keeps its formatting**, so a copied list, heading, or bold and italic text arrives with its structure intact rather than flattened. A pasted image becomes an image block there. This is the fast path for dropping a screenshot exactly where you want it.

## Copy a text block's text

**Hover a text block** and a small **copy button** appears in its upper-right corner, next to the collapse and delete controls. Click it to copy the block's text to your clipboard as **markdown** — headings, bold and italic, links, and nested lists come across as markdown, so the text pastes cleanly into another editor, a chat message, or another Notus block. An empty block shows no copy button.

This copies the *text*. To copy the *block itself* — to duplicate it elsewhere on the canvas, keeping it as a block — select it and use Ctrl+C (Cmd+C on macOS), or **Copy** from its right-click menu.

## Move and resize

- **Move a block** by dragging its edge. (Clicking *inside* a text block puts your cursor in the text instead of moving the block — drag the edge to move it.)
- **Resize a block** by dragging the handles that appear when it is selected. Most blocks resize from their **left and right edges**; a text block's height follows its text, and a sticky note can also be made taller from its bottom edge. **Images** resize from their **corners** and keep their proportions; hold **Shift** to stretch one freely. **Shapes** have handles on every corner and edge.

### Keep blocks from overlapping

Turn on **Settings → Editing → Keep blocks from overlapping** and a block you drop on top of another **slides to the nearest free space** when you let go. It follows the pointer exactly while you drag; it only settles on release. **Hold Option (Alt on Windows) while you let go** to place it exactly where it is, overlap and all. The setting is **off** until you turn it on.

- **A group** you drag together moves as one: the whole group slides by the same amount, so the blocks keep their arrangement.
- **Pasting, Duplicate and the toolbar's insert buttons** also land a new block on free space, and so do blocks an agent or a Coding Session adds or moves.
- **Shapes never slide, and nothing slides off them** — shapes are meant to be drawn over blocks. Arrows and blocks you've hidden from the agent don't count either.
- **Inside a container**, a block only avoids the other blocks in that container. Dropping a block *into* a container places it the usual way.
- Only the block you moved moves: nothing else is pushed aside, and turning the setting on doesn't rearrange blocks that already overlap.
- **Cmd+Z** (Ctrl+Z) puts a block that slid back where it was before you dragged it, in one step.

**The first block on an empty page** — added with a toolbar button or by an agent — lands a little in from the top-left corner rather than flush against it. A block you place by clicking or drawing still goes exactly where you put it.

## Select several blocks

**Drag a box** across empty canvas to select blocks — a "rubber-band" selection. A block is selected when the box fully encloses it: clipping a corner is not enough, the whole block has to be inside. (Holding **Ctrl**, or **Cmd** on macOS, while you drag does the same thing, so the older habit still works.) Dragging any selected block by its move handle then moves the whole group together, keeping their arrangement.

You can also **copy a selection** with Ctrl+C (Cmd+C on macOS) and paste it with Ctrl+V (Cmd+V) — on the same page, another page, or even another notebook. The blocks land with their arrangement intact, and any arrows connecting the selected blocks come along and stay attached to the copies.

**Right-click → Copy does the same thing.** With several blocks selected, right-clicking any one of them and choosing **Copy** copies the whole selection — not just the block under the pointer — including the arrows between them. Right-clicking a block that is *not* part of the selection copies just that block, which is what you would expect from aiming at it.

## Pan and zoom

- **Pan** the page by **holding the spacebar and dragging**. This is the one that works on every mouse and trackpad — a Magic Mouse and a MacBook trackpad have no middle button — and it works anywhere on the canvas, over a block as well as empty space, and while a drawing tool is selected. Let go of the spacebar and dragging goes back to selecting.
- **If your mouse has a middle button**, dragging with it pans the same way, with no key to hold.
- **On Windows** you can also hold the **right** mouse button and drag. A right-click without dragging still opens the menu. You can turn this off in **Settings → Editing**.
- **Or just scroll** — a mouse wheel or two fingers on a trackpad moves the page in any direction (vertical and horizontal both work), with no button and no key at all.
- **Zoom** by holding **Ctrl** (or **Cmd** on macOS) and scrolling, by pinching on a trackpad, or with the zoom controls in the page toolbar. Zoom runs from **25% to 400%**.

Each page remembers its own pan position and zoom level between sessions. If you get lost, use **View → Reset Zoom** (**Ctrl+0**, or **Cmd+0** on macOS, or the middle button of the zoom controls): it returns the page to 100% and to its top-left corner.

Some blocks hold more than they can show at once — an MQTT topic tree, a knowledge-graph payload, an AI agent's transcript, a long imported document.

**Point at the part you want and scroll.** Anything with its own scrolling area takes the scroll directly, with no click and no modifier key: a dropdown or menu, the conversation list and message stream in a Slack or Email block, a calendar grid, query results (sideways too, for a wide result set), and an agent's code and tool-output panels.

**For a block with a single scrolling body — an agent transcript, an imported document, an audit log — click the block once to focus it, then scroll from anywhere on the page** and that block's content moves instead of the canvas.

## More room for the canvas

For an even bigger workbench, hide the toolbars above the canvas with **View → Toggle Toolbars** (Ctrl+Shift+\\, or Cmd+Shift+\\ on macOS). The page title and the Back/Forward buttons stay on a slim bar with a chevron you can click to bring the toolbars back, and the setting is remembered between sessions. (This is separate from **Toggle Sidebar** — you can hide either, or both.)

When the window is narrow — or the sidebar is dragged out wide — the row of block-insert buttons on the right of the second toolbar may not have room for all of them. The ones that don't fit fold into a **»** menu at the end of the row, starting from the right-hand end, so the buttons you reach for most often stay out where you can click them. Click **»** to see the rest: every button that isn't in the row is in that menu, with the same icon and the same name. Widen the window or narrow the sidebar and they come back out on their own.

The **»** appears only when something has actually folded away, so it takes no space when everything fits. The **Connectors** button and the **?** formatting-help button never fold into the menu — they stay at the end of the row, after the **»**.

**Narrower still, the drawing tools on the left fold the same way.** Shapes and Components go first, then the line styles, stroke weights and colors, so the drawing tools themselves stay out longest. Whatever has folded moves behind a **⋯** button at the end of the drawing tools — a different symbol from the **»** on the right, so the two are easy to tell apart. The **⋯** panel holds the real controls rather than a list of commands, so it **stays open** while you pick a color and then a line weight. The zoom controls never fold, and neither do **Connectors** and **?** — between them that is what keeps every one of those reachable right down to the smallest window Notus will open. (The one exception is a sidebar dragged out very wide on a very small window — if the row still runs out of room, narrow the sidebar and everything comes back.)

## Stacking order

Every object's right-click menu — a block, or a shape or line inside a diagram — follows the same order: the object's own actions first, then appearance (such as **Styling**), then arrangement (**Z-Order**, **Align**), then **Copy** and **Duplicate**, then **Hide from agent**, then **Info**, with **Delete** always at the bottom. Thin lines separate the groups, and an object only shows the groups it has.

Because blocks can overlap, each one has a front-to-back order. Right-click a block and open **Z-Order** to move it: **Bring to Front**, **Bring Forward**, **Send Backward**, or **Send to Back**. An option is greyed out when the block is already as far in that direction as it can go.

**Inside a container, these move the block among the others in that same frame.** Blocks elsewhere on the page are not involved, and **Send to Back** stops at the container's own frame rather than going behind it — so a block sent to the back of a container stays visible, tucked behind its neighbors but in front of the frame.

## Delete and undo

- Select one or more blocks and press **Backspace** or **Delete** to remove them.
- **Undo** with Ctrl+Z (Cmd+Z on macOS); **redo** with Ctrl+Shift+Z. Undo covers everything on the page — creating, moving, resizing, and deleting blocks, as well as text edits — so you can step back through your changes in order. Undo history belongs to the page you are on and lasts for this session: switching to another page, or quitting Notus, starts a fresh history.

Next, learn how to find your notes again in [Finding things](04-finding-things.md).
