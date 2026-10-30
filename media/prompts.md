# Media prompts (v0.1, 2026-10-30)

Each element is made with the tool that does that job best, then credited on the page. Keep a note of the exact tool and date for every file you make, so the credit table stays true.

Drop finished files in `media/`. Any size is fine; Claude Code will compress them for the page.

## 1. Images: ChatGPT (image generation)

Style block to put at the start of every image prompt:

> Flat vector illustration. Soft indigo and blue palette with warm yellow accents, clean simple shapes, generous empty space. No text, no letters, no logos, no real people and no realistic faces (simple abstract figures are fine). 16:9.

**hero.png**
> A friendly open toolbox on a desk. Instead of hammers, the tools are a terminal window, a branching diagram like a subway map, a chat bubble, a magnifying glass over a page of code, and a shield with a checkmark. A laptop glows softly in the background.

**tools.png**
> A pegboard wall with nine different tools hung in a tidy grid, each a different shape and accent colour: a pen, a magnifier, an open book, a lightning bolt, a stack of papers, a globe, a chat bubble, a small window, and a shield. Warm lighting.

**git.png**
> A subway-map style diagram of a software project's history: one main line with several short branches splitting off and merging back, small circles for each change, and one branch ending in a small undo arrow. Calm and clean.

**judgment.png**
> A simple abstract figure at a desk holding up a calm hand to pause a friendly robot arm that is offering a glowing page of code. The figure is clearly in control. No faces.

Alt text to use on the page:
- hero: A toolbox filled with digital tools: a terminal, a branching diagram, a chat bubble and a shield.
- tools: A pegboard with nine different tools, each one suited to a different job.
- git: A subway-style map of a project's history, with branches splitting and merging.
- judgment: A person pausing a robot arm that is offering code.

## 2. Video: NotebookLM (video overview)

1. Go to notebooklm.google.com and create a new notebook.
2. Upload only `media/notebooklm-source.md`.
3. In the Studio panel choose **Video Overview**.
4. Style: choose **Custom** and paste the style line below. (Custom styles are for adults, which you are.) If Custom isn't offered, pick **Whiteboard** or **Paper-craft**.
5. Paste the steering prompt below.
6. Generate. It can take 30 minutes or more. Then use **Download** in the player.

Style line:
> Clean flat vector illustration with a soft indigo and blue palette and warm yellow accents, calm and professional, no cartoon faces.

Steering prompt:
> Audience: a school principal and teachers deciding whether to offer an after-school club. Keep it short, about 90 seconds if the length can be set. Tone: calm, confident, no hype. Cover: the gap (students learn Python but not the newest AI coding tools or how to check them), the right tool for the job, git typed by hand, the human in the loop (the AI drafts, a person decides), and the guardrails (ages 13 and over, parent or guardian consent, tools the school allows). Do not mention prices or any commercial plans. Do not invent facts that are not in the source.

Save as `media/overview.mp4`. Keep it under about 20 MB (Claude Code can compress it). Review it end to end before it goes on the page.

## 3. Animation: Claude (normal chat on your Pro plan)

Claude Motion needs a Team or Enterprise plan, so use an animated Artifact in a normal chat instead. It is the same idea (Claude writes code that animates text and shapes) without the MP4 export. Paste this into a new Claude chat:

> Build a single self-contained HTML file: a short animated explainer of about 60 seconds, five scenes, no external libraries, fonts or images. Colours: indigo (#2f5bea), soft blue (#eef2ff), warm yellow accent, dark text on light, and a dark mode that follows prefers-color-scheme. Scenes, each with one short caption and one simple animated shape: (1) "Students already use AI tools." (2) "Few are taught which one to reach for." (3) "Right tool for the job." Show nine small tool shapes sliding into a toolbox. (4) "Git, typed by hand." Show a line of commits that branches and merges. (5) "A human decides." Show a hand pausing a robot arm, then a checkmark. Include play, pause and replay buttons that work with the keyboard. If prefers-reduced-motion is on, show the five scenes as static panels instead. Keep the file under 100 KB.

Save the result as `media/explainer.html`. It can be added to the page as a self-hosted block, so no outside site is needed.

Alternative if you want an MP4 instead: Remotion (open source) makes video from code, and Claude Code can build the project, but it needs more setup.

## 4. Voiceover: ElevenLabs (optional, can skip for now)

Skip this for the first media version if you want it simple: the explainer works with captions, and the NotebookLM video already has voices. Add narration only if you want a spoken version.

Whose voice: ElevenLabs offers a library of stock AI voices you pick from, and it can clone a voice from a sample. Cloning is on paid plans, and you may only clone your own voice or someone who has given written consent. Never clone anyone else's.

Licensing: the free plan does not include commercial use. A pitch for a club that may become paid work is a grey area, so use one month of a paid plan or skip it.

Recommendation: pick a calm, clear stock voice (not an energetic "advert" voice), or record yourself. Note the voice name for the credit.

Script (about 75 seconds):
> Students are taught Python, which is fundamental and current. But they are not taught how the newest AI coding tools work, which one to reach for, or how to tell when the answer is wrong. They are using these tools anyway, mostly on their own. This club gives them habits. They learn that different tools are good at different jobs. They learn git, typed by hand, the developer's safety net. And they learn the most important skill of all: judgment. Knowing when to push back on a tool. The AI drafts. A person decides. Students must be thirteen or over, with a parent or guardian's consent where a tool requires it, and only tools the school allows. If you are curious what students could make, you are looking at an example.

Save as `media/voiceover.mp3`.

## Credits to add once each exists

| Element | Credit line |
|---|---|
| Images | Images made by ChatGPT (image generation), prompts by Mark |
| Video | Video overview made by NotebookLM from a source text written with Claude and approved by Mark |
| Animation | Animated explainer written by Claude in a chat, reviewed by Mark |
| Voiceover | Voice: [ElevenLabs voice name], script approved by Mark |
