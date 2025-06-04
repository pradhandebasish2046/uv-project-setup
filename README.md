# MyProject Setup

```bash
curl -Ls https://astral.sh/uv/install.sh | bash
export PATH="$HOME/.cargo/bin:$PATH"
source ~/.bashrc
uv --version

mkdir myproject && cd myproject
uv venv
source .venv/bin/activate
uv add numpy
uv sync
uv lock

# Tu run ipynb
uv add --dev ipykernel
