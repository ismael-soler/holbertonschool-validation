build: ## Generates the website from a markdown file
	hugo

clean: ## Cleans the content of the directory dist
	rm -fr dist

post: ## Creates a post with a given name and title
	hugo new posts/$(POST_NAME).md
	sed -i '/title/c\title: "$(POST_TITLE)"' content/posts/$(POST_NAME).md

help:	## some help
	@fgrep "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/##//'