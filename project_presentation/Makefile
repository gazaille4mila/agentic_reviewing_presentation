.PHONY: help install clean build-presentation build-all

help: ## Show this help message
	@awk -F':.*?## ' '/^[a-zA-Z0-9_-]+:.*## / {printf "\033[36m%-20s\033[0m %s\n", $$1, $$2}' $(MAKEFILE_LIST)

install: ## Install LaTeX and Work Sans on macOS (Homebrew)
	@if ! command -v brew >/dev/null 2>&1; then \
		echo "Homebrew is required for 'make install': https://brew.sh"; \
		exit 1; \
	fi
	@if command -v latexmk >/dev/null 2>&1 && command -v xelatex >/dev/null 2>&1; then \
		echo "LaTeX toolchain already installed (latexmk + xelatex). Skipping MacTeX."; \
	else \
		brew install --cask mactex; \
	fi
	@if brew list --cask font-work-sans >/dev/null 2>&1; then \
		echo "Work Sans already installed via Homebrew. Skipping font installation."; \
	else \
		brew install --cask font-work-sans || { \
			echo "Could not install Work Sans via Homebrew."; \
			echo "Install it manually from: https://fonts.google.com/specimen/Work+Sans"; \
			exit 1; \
		}; \
	fi

clean: ## Nuke build artifacts
	rm -f presentation.pdf
	rm -f *.aux *.bbl *.bcf *.blg *.log *.out *.run.xml *.toc *.lof *.lot
	rm -f *.nav *.snm *.synctex.gz *.fdb_latexmk *.fls *.xdv

build-presentation: ## Build the presentation deck
	latexmk -pdfxe presentation.tex

build-all: clean build-presentation ## Clean and build everything
