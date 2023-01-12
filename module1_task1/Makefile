build:
	hugo

clean:
	rm -fr dist

post:
	hugo new posts/$(POST_NAME).md
	sed -i '/title/c\title: "$(POST_TITLE)"' content/posts/$(POST_NAME).md