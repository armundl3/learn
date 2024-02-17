# Variables
PYTHON_VERSION := 3.9.7
VENV := venv
PYTHON := $(VENV)/bin/python$(PYTHON_VERSION)
PIP := $(VENV)/bin/pip

# Targets
.PHONY: all clean

all: $(VENV) install_requirements

$(VENV):
	virtualenv -p python$(PYTHON_VERSION) $(VENV)

install_requirements: $(VENV)
	$(PIP) install -r requirements.txt

clean:
	rm -rf $(VENV)
