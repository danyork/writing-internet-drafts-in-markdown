#
# Makefile to build Internet Drafts from markdown using mmarc and
# relying on the docker image "paulej/rfctools".
#

SRC  := $(wildcard draft-*.md)
TXT  := $(patsubst %.md,%.txt,$(SRC))
UID  := `id -u`
GID  := `id -g`
CWD  := `pwd`

# Ensure the xml2rfc cache directory exists locally
IGNORE := $(shell mkdir -p $(HOME)/.cache/xml2rfc)

all: $(TXT) $(HTML)

clean:
	rm -f draft*.txt draft-*.xml

%.txt: %.md
	docker run --rm --user=$(UID):$(GID) -v $(CWD):/rfc -v $(HOME)/.cache/xml2rfc:/var/cache/xml2rfc paulej/rfctools md2rfc $^
