# uv-project-setup
curl -Ls https://astral.sh/uv/install.sh | bash
export PATH="$HOME/.cargo/bin:$PATH"
source ~/.bashrc  # reload the shell
uv --version  # verify the version

mkdir myproject && cd myproject
uv venv
source .venv/bin/activate
uv add numpy
uv sync
uv lock
