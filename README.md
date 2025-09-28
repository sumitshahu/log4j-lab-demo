
## What this repo is

I created this repo to demonstrate a vulnerable Java web application and a proof-of-concept exploit that shows how the vulnerability can be triggered. It’s meant as a learning example so you can see how the issue works and why it's dangerous.

---

## What’s inside

* **A simple vulnerable web application (Java)** that demonstrates how Log4j can be abused.
* **`poc.py`** — a demonstration script that automates the exploit flow for study and testing in a lab environment.
* **`Dockerfile`** — to build and run the vulnerable app in an isolated container.
* **Example files and small helper scripts** used by the demo.

---

## Requirements

* **Python 3** (to run `poc.py` and other helpers)
* **Docker** (to build and run the vulnerable web application in a container)
* Basic command-line tools (bash / PowerShell)

---

## Quick setup — build and run the vulnerable app (Docker)

1. Build the Docker image from the project folder:

```bash
docker build -t log4j-shell-poc .
```

2. Run the container (this example uses host networking for simplicity; on some systems you may need different flags):

```bash
docker run --network host log4j-shell-poc
```

3. Open your browser and visit `http://localhost:8080` (or the port shown by the container) to interact with the demo app.

---

## Running the demonstration script (`poc.py`)

1. Install Python requirements:

```bash
pip install -r requirements.txt
```


2. Run the script from the project folder (example):

```bash
python3 poc.py --help
```

## Files overview

* `Dockerfile` — builds the vulnerable web application image
* `poc.py` — PoC demonstration script (Python)
* `README.md` — this file
* Other helper scripts and resource files used in the demo

---
