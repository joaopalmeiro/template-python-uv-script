# Template Notes

- Zed:
  - [EditorConfig](https://github.com/zed-industries/zed/issues/8534) issue
  - [Top-Ranking Issues (All Time)](https://github.com/zed-industries/zed/issues/5393) issue
  - https://zed.dev/docs/telemetry
  - https://zed.dev/docs/configuring-zed
  - https://github.com/zed-industries/zed/releases
  - Current global configuration: https://github.com/joaopalmeiro/dotfiles
- Ruff:
  - https://github.com/astral-sh/ruff/issues/809
  - https://github.com/astral-sh/ruff/discussions/3363
  - https://github.com/astral-sh/ruff/issues/1530
  - https://github.com/astral-sh/ruff/releases
  - [`docs`: remove `.` from check and format commands](https://github.com/astral-sh/ruff/pull/10217)
  - https://github.com/astral-sh/ruff?tab=readme-ov-file#usage
  - https://github.com/astral-sh/ruff/releases/tag/v0.3.5:
    - "[`flake8-boolean-trap`] Add setting for user defined allowed boolean trap"
  - https://docs.astral.sh/ruff/rules/#refurb-furb
  - https://pypi.org/project/refurb/
  - https://astral.sh/blog/ruff-v0.4.0
  - https://astral.sh/blog/ruff-v0.6.0
  - https://github.com/astral-sh/ruff/releases/tag/0.14.11
  - https://docs.astral.sh/ruff/settings/#lint_typing-extensions
  - https://astral.sh/blog/ruff-v0.15.0
    - https://docs.astral.sh/ruff/formatter/#markdown-code-formatting (preview)
- uv:
  - https://github.com/astral-sh/uv?tab=readme-ov-file#python-discovery
  - https://github.com/astral-sh/uv/releases
  - https://github.com/astral-sh/uv/blob/0.1.17/PIP_COMPATIBILITY.md
  - `uv pip check`:
    - https://github.com/astral-sh/uv/blob/0.1.24/PIP_COMPATIBILITY.md
    - [Add `uv pip check`](https://github.com/astral-sh/uv/pull/2397)
    - https://github.com/astral-sh/uv/blob/0.1.24/PIP_COMPATIBILITY.md#pip-check
    - https://pip.pypa.io/en/stable/cli/pip_check/
  - https://github.com/astral-sh/uv/releases/tag/0.1.30:
    - https://github.com/astral-sh/uv/blob/0.1.30/crates/uv/Cargo.toml#L49
    - https://crates.io/crates/miette
  - `uv.toml`:
    - https://github.com/astral-sh/uv/blob/0.1.39/PIP_COMPATIBILITY.md#configuration-files-and-environment-variables
    - https://github.com/astral-sh/uv/issues/651
  - https://github.com/astral-sh/uv/pull/3859: `uv pip tree`
  - https://github.com/astral-sh/uv/pull/5141: https://github.com/oracle/graalpython
  - https://docs.astral.sh/uv/
  - https://docs.astral.sh/uv/getting-started/installation/#homebrew
  - https://github.com/astral-sh/uv/releases/tag/0.3.0:
    - "`uv venv` will read the required Python version from the `.python-version` file or `pyproject.toml`"
  - `uvx` or `uv tool run`:
    - Alternative to `pipx`
    - "Tools are Python packages that provide command-line interfaces."
  - "The pip interface": "uv provides a drop-in replacement for common `pip`, `pip-tools`, and `virtualenv` commands."
  - https://docs.astral.sh/uv/guides/publish/: "uv does not yet have dedicated commands for building and publishing a package."
  - https://docs.astral.sh/uv/concepts/python-versions/:
    - "uv does not distinguish between Python versions installed by the operating system vs those installed and managed by other tools. For example, if a Python installation is managed with `pyenv`, it would still be considered a _system_ Python version in uv."
    - `uv python install`: "However, a project may define a `.python-version` file specifying the default Python version to be used. If present, uv will install the Python version listed in the file."
  - https://docs.astral.sh/uv/reference/settings/:
    - https://docs.astral.sh/uv/reference/settings/#exclude-newer: "Limit candidate packages to those that were uploaded prior to the given date."
  - https://docs.astral.sh/uv/concepts/python-versions/#python-implementation-support:
    - "uv supports the CPython, PyPy, and GraalPy Python implementations."
    - "uv supports downloading and installing CPython and PyPy distributions."
  - https://docs.astral.sh/uv/pip/packages/#installing-packages-from-files
  - https://docs.astral.sh/uv/pip/dependencies/#using-requirementsin: `requirements.in` instead of `requirements.txt`
  - https://github.com/astral-sh/uv/releases/tag/0.3.1
  - https://docs.astral.sh/uv/reference/settings/#managed
  - https://docs.astral.sh/uv/reference/settings/#package
  - [`uv` should provide a build backend](https://github.com/astral-sh/uv/issues/3957) open issue
  - https://docs.astral.sh/uv/guides/publish/#building-your-package
  - https://docs.astral.sh/uv/guides/publish/#publishing-your-package
  - https://docs.astral.sh/uv/guides/scripts/#creating-a-python-script
  - [Add templates for popular build backends](https://github.com/astral-sh/uv/pull/7857) PR
  - https://docs.astral.sh/uv/concepts/projects/dependencies/#default-groups: "By default, uv includes the `dev` dependency group in the environment (...)"
  - https://docs.astral.sh/uv/configuration/files/#env: `uv run --env-file .env -- python -c 'import os; print(os.getenv("MY_VAR"))'`
  - https://bas.codes/posts/python-project-setup-uv
  - https://docs.astral.sh/uv/concepts/projects/sync/
- File nesting:
  - https://code.visualstudio.com/updates/v1_67#_explorer-file-nesting
  - https://github.com/antfu/vscode-file-nesting-config?tab=readme-ov-file#update-manually:
    - Example: `"Pipfile": ".editorconfig, .flake8, .isort.cfg, .python-version, Pipfile, Pipfile.lock, requirements*.in, requirements*.pip, requirements*.txt, tox.ini"`
  - https://code.visualstudio.com/docs/getstarted/settings#_default-settings:
    - Example: `"package.json": "package-lock.json, yarn.lock, pnpm-lock.yaml, bun.lockb"`
  - PyCharm also supports file nesting: https://www.jetbrains.com/help/pycharm/file-nesting-dialog.html
- mypy:
  - https://pypi.org/project/mypy/
  - https://github.com/python/mypy/blob/master/CHANGELOG.md#mypy-110
  - https://github.com/python/mypy/blob/master/CHANGELOG.md#mypy-111:
    - "Mypy now type checks uses of `functools.partial`."
  - https://github.com/python/mypy/blob/master/CHANGELOG.md#mypy-112:
    - "Mypy now always tries to infer a union type for a conditional expression if left and right operand types are different. This results in more precise inferred types and lets mypy detect more issues."
    - "You can now use `typing.ReadOnly` to specity `TypedDict` items as read-only (...)"
    - https://docs.python.org/3/library/typing.html#typing.ReadOnly: "Added in version 3.13."
    - https://github.com/python/mypy/blob/master/CHANGELOG.md#experimental-inline-typeddict-syntax
  - Config source:
    - https://github.com/pydantic/pydantic/blob/v2.6.3/docs/integrations/mypy.md#configuring-the-plugin
    - https://github.com/FlorianWilhelm/the-hatchlor/blob/v0.3/%7B%7Bcookiecutter.project_slug%7D%7D/pyproject.toml#L81
    - https://github.com/python/mypy/blob/1.9.0/docs/source/config_file.rst
    - https://github.com/python/mypy/blob/1.9.0/docs/source/config_file.rst#example-mypyini
    - https://github.com/python/mypy/blob/1.9.0/docs/source/existing_code.rst#introduce-stricter-options
    - https://github.com/python/mypy/blob/master/CHANGELOG.md#mypy-19
- https://github.com/RustPython/Parser
- https://github.com/RustPython/RustPython
- https://github.com/youknowone/baembal
- https://www.python.org/downloads/
- https://github.com/dimastbk/python-calamine
- https://www.stefanjudis.com/today-i-learned/readonly-files-in-vscode/
- https://blog.yusong.me/config/vscode
- https://code.visualstudio.com/docs/editor/glob-patterns
- https://mac.install.guide/homebrew/4
- Scripton:
  - Python IDE
  - https://scripton.dev/
  - https://docs.scripton.dev/ide/manual/visualization
- https://github.com/NowanIlfideme/pydantic-yaml
- https://docs.swarms.world/en/latest/swarms/structs/yaml_model/
- GEPA:
  - https://pydantic.dev/articles/prompt-optimization-with-gepa
  - https://github.com/Studio-Intrinsic/benchmarking-ocr-gepa
  - https://github.com/gepa-ai/gepa
    - "The easiest and most powerful way to use GEPA for prompt optimization is within DSPy, where the GEPA algorithm is directly available through the `dspy.GEPA` API."
    - https://github.com/gepa-ai/gepa/blob/v0.0.27/src/gepa/examples/aime.py
    - https://huggingface.co/datasets/AI-MO/aimo-validation-aime
    - It supports multimodal tasks: https://github.com/gepa-ai/gepa/blob/b2b613ea189e72867d085b93614b3e626e4ccd8b/docs/docs/guides/faq.md#can-gepa-work-with-multimodalvlm-tasks
    - https://gepa-ai.github.io/gepa/
    - https://gepa-ai.github.io/gepa/guides/quickstart/#option-1-using-the-default-adapter
      - `# Prepare data (aim for 30-300 examples for best results)`
  - https://dspy.ai/tutorials/gepa_aime/
  - https://dspy.ai/tutorials/gepa_facilitysupportanalyzer/
  - https://huggingface.co/learn/cookbook/en/dspy_gepa
  - https://dspy.ai/learn/programming/signatures/?h=image#example-e-multi-modal-image-classification

## Commands

```bash
rm -rf deprecated/ TEMPLATE.md
```

```bash
zed ~/Documents/GitHub/template-python-uv-script/
```

```bash
uv --help
```

```bash
uv venv --help
```

```bash
uv pip install --help
```

```bash
uv pip list --help
```

```bash
which ruff
```

```bash
uv pip check --help
```

```bash
uv pip sync requirements.txt
```

```bash
uv pip sync --reinstall --refresh --strict requirements.txt
```

```bash
ruff check --show-settings
```

```bash
ruff check --show-files
```

```bash
which ruff && which mypy
```

```bash
uv tool --help
```

```bash
uv python pin 3.10.13
```

```bash
brew install uv
```

```bash
brew update
```

```bash
brew upgrade uv
```

```bash
uv cache prune
```

```bash
uv cache clean
```

```bash
uv pip list --format json
```

```bash
pip config unset global.require-virtualenv
```

```bash
uv python list
```

```bash
uv init --script example.py --python 3.10
```

```bash
ruff check
```

## Snippets

```python
import dspy
from dspy.teleprompt.gepa.instruction_proposal import MultiModalInstructionProposer

lm = dspy.LM("openai/gpt-4o-mini", api_key=api_key)
dspy.configure(lm=lm)


# Define the signature
class ImageQA(dspy.Signature):
    """Answer the question based on the image."""

    image: dspy.Image = dspy.InputField(desc="An image to analyze")
    question: str = dspy.InputField()
    answer: str = dspy.OutputField()


# Instantiate the program
program = dspy.Predict(ImageQA)


# Define the metric with feedback
def metric_with_feedback(example, prediction, trace=None):
    correct = example.answer.lower() in prediction.answer.lower()
    score = 1.0 if correct else 0.0

    if correct:
        feedback = f"Correct! The answer '{prediction.answer}' matches the expected answer '{example.answer}'."
    else:
        feedback = (
            f"Incorrect. Expected '{example.answer}' but got '{prediction.answer}'. "
            f"Look more carefully at the visual content in the image."
        )

    return dspy.Prediction(score=score, feedback=feedback)


# Prepare the dataset
trainset = [
    dspy.Example(
        image=dspy.Image("https://example.com/photo_of_eiffel_tower.jpg"),
        question="What landmark is shown?",
        answer="Eiffel Tower",
    ).with_inputs("image", "question"),
    dspy.Example(
        image=dspy.Image("/path/to/local/cat_image.png"),
        question="What animal is in the image?",
        answer="cat",
    ).with_inputs("image", "question"),
    # ... more examples (aim for 30-300)
]


# Optimize with GEPA
optimizer = dspy.GEPA(
    metric=metric_with_feedback,
    reflection_lm=dspy.LM("openai/gpt-4o", api_key=api_key),
    instruction_proposer=MultiModalInstructionProposer(),
    auto="light",
    num_threads=8,
    track_stats=True,
)

optimized_program = optimizer.compile(program, trainset=trainset)


# View the optimized prompt
print(optimized_program.signature.instructions)
```

```python
import dspy
from datasets import load_dataset
from dspy.teleprompt.gepa.instruction_proposal import MultiModalInstructionProposer

api_key = input("Enter your OpenAI API key: ")

lm = dspy.LM("openai/gpt-4o-mini", api_key=api_key)
dspy.configure(lm=lm)


# Define the signature
class ChartQA(dspy.Signature):
    """Answer the multiple-choice question about the chart. Respond with only the letter of the correct option."""

    image: dspy.Image = dspy.InputField(desc="A chart or visualization")
    question: str = dspy.InputField()
    options: str = dspy.InputField(desc="The available answer options")
    answer: str = dspy.OutputField(desc="The letter of the correct option (A, B, C, or D)")


# Instantiate the program
program = dspy.Predict(ChartQA)


# Load and prepare the dataset
def init_dataset():
    ds = load_dataset("joaompalmeiro/MiniVLATGHDataset", split="test")

    examples = []
    for row in ds:
        opts = row["options"]
        options_str = ", ".join(
            f"{k}: {v}" for k, v in opts.items() if v is not None
        )

        examples.append(
            dspy.Example(
                image=dspy.Image(row["image"]),
                question=row["question"],
                options=options_str,
                answer=row["answer"],
            ).with_inputs("image", "question", "options")
        )

    return examples


trainset = init_dataset()
print(f"Loaded {len(trainset)} examples")


# Define the metric with feedback
def metric_with_feedback(example, prediction, trace=None):
    correct = prediction.answer.strip().upper() == example.answer.strip().upper()
    score = 1.0 if correct else 0.0

    if correct:
        feedback = f"Correct! The answer '{prediction.answer}' matches the expected answer '{example.answer}'."
    else:
        feedback = (
            f"Incorrect. Expected '{example.answer}' but got '{prediction.answer}'. "
            f"Look more carefully at the visual content in the chart. "
            f"The options were: {example.options}."
        )

    return dspy.Prediction(score=score, feedback=feedback)


# Optimize with GEPA
optimizer = dspy.GEPA(
    metric=metric_with_feedback,
    reflection_lm=dspy.LM("openai/gpt-4o", api_key=api_key),
    instruction_proposer=MultiModalInstructionProposer(),
    auto="light",
    num_threads=8,
    track_stats=True,
)

optimized_program = optimizer.compile(program, trainset=trainset)

# View the optimized prompt
print(optimized_program.signature.instructions)
```
