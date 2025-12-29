# Project info
- project.md has a summary of the project and planned work
- reference/ folder has a summary of reference Llama_Omni2 paper we're following and some files from their github

# Guidelines
- Keep in mind that the user is brand new to model training. Provide a succinct 'why' and explain what you are trying to achieve before implementing anything. Help the user learn the process and grasp key technical details along the way.
- Think through the approach before writing any code. If there are key decisions or clarifications needed, make recommendations and check in before implementing. The goal is the simplest cleanest correct end state.
- When implementing, go step by step methodically, don't just one-shot a big chunk of code in one go. Avoid bloat, avoid useless wrappers, avoid premature scaffolding, prefer tiny, clean, organized, easy to understand, and lightweight solutions.
- If something is messy, hacky, or wrong, flag it and propose the clean fix. Don’t stack more bad code on top.
- Make sure code is clean, easy to parse and understand, like Andrej Karpathy's ML open source projects. Include well-formatted comments where they are useful for understanding (e.g. top of key modules, sections, functions).
- Use pytorch, or Huggingface Transformers, Accelerate, and Datasets libraries if they have the appropriate functions vs. re-inventing the wheel. Let Accelerate manage devices and types unless there's a specific need to customize.
- Don't be limited by your constraints like lack of network access or inability to run a file. These do not apply to the user. Consider the user your partner with access to everything, if you need something done, ask the user to do it.
- Always run models on GPU/cuda by default, never CPU. Avoid setting configs that don't need be set, where the defaults are fine.
- Assume anything done locally will eventually be run on cloud rented GPUs.
- We are using a python venv, keep this in mind when running python commands or scripts.
- Always be clear on the critical things you are trying to validate when writing tests. Keep tests clean, simple, and reflective of real use. No faked, mocked, or useless tests that are just there to get passed. Tests should not fail or skip silently.
