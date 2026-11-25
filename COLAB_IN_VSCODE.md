# Work in VS Code with a Colab kernel

This checkout is your fork: https://github.com/Sal-Faris/sain-coursework.

## Open your coursework

1. In VS Code, open this **sain-coursework** folder with **File > Open Folder**.
2. Open `technical/evaluations/Assignment_1_Intro_to_Evals.ipynb` to continue the course assignment. Your recovered code through the alignment-faking exercise is filled in. The discussion, threat-modeling and question-design exercises are still yours to complete.
3. At the notebook's top right, choose **Select Kernel > Colab > Auto Connect**. Sign in to Google if prompted. The official **Google Colab** and **Jupyter** extensions are already installed on this computer.
4. Run the setup cells, then work down the notebook. Packages and data are prepared inside the Colab runtime. You do not need a local Python environment or Google Drive storage.
5. In the API-client cell, an existing `OPENROUTER_API_KEY` environment variable or Colab secret is used when available. Otherwise enter your key into the hidden input prompt. Keep the key out of code cells and outputs.

The earlier ARENA notebook at `chapter3_llm_evals/exercises/part1_intro_to_evals/3.1_Intro_to_Evals_exercises.ipynb` has the same recovered code and Colab setup if you prefer its original chapter layout. Use the assignment notebook for the course's answer slots.

## Save to GitHub

1. Press **Ctrl+S** to save notebook edits and outputs to this local checkout.
2. Open **Source Control** (Ctrl+Shift+G), review your changes, and click **+** to stage the files you want to save.
3. Enter a message such as `Restore intro to evals work` and choose **Commit**.
4. Choose **Push** (or **Sync Changes**) to save the commit to `Sal-Faris/sain-coursework`.

Ctrl+S saves locally. Git commit and push save a version on GitHub. Colab disconnecting does not delete this local notebook, but variables and packages in the remote runtime must be recreated by running setup again.

## Runtime and data

The notebook file lives on this laptop; Python executes on Google's Colab server. Paths in executed code refer to the server's filesystem, not the laptop. Setup downloads the exercise data from ARENA when the runtime cannot see the bundled copy. The prompt files and queries are also included in this repository for reference and local use. Changes to those local data files are not automatically uploaded to a remote Colab runtime.

The recovered replication cell sends 40 API calls at `N_PROMPTS = 20`. API example cells also make requests when run. Restore the code first and run the paid API cells when you are ready. No experiment results have been fabricated or filled in.

Official extension instructions: https://marketplace.visualstudio.com/items?itemName=Google.colab

Exercise assets: https://github.com/ARENA-education/ARENA_materials/tree/main/chapter3_llm_evals/exercises/part1_intro_to_evals
