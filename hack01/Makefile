.PHONY: makelib

FILE := sample.cry
KEY := easy

makelib:
	gcc bypassauth.c -m32 -shared -fPIC -o bypassauth.so

run:
	echo -e "test\ntest\n" | LD_PRELOAD=bypassauth.so ./docrypt $(FILE) $(KEY)

clean:
	rm bypassauth.so