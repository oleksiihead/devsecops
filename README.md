# pre-commit for gitleaks

## Junior

Install gitleaks for your OS and check gitleaks version
```
# MacOS
brew install gitleaks
# From Source for Linux
git clone https://github.com/gitleaks/gitleaks.git
cd gitleaks
make build
sudo ln -s /path/to/gitleaks /usr/local/bin/gitleaks
gitleaks version
```

Clone this repo and create pre-commit for gitleaks
```
git clone <repo_url>
cp <repo_dir>/pre-commit-examples/pre-commit-junior .git/hooks/pre-commit
chmod +x .git/hooks/pre-commit
```
Now you can commit your code as usual and use advantages of the gitleaks

```
git commit -m "Check gitleaks"

    ○
    │╲
    │ ○
    ○ ░
    ░    gitleaks

10:39AM INF 1 commits scanned.
10:39AM INF scan completed in 63.7ms
10:39AM INF no leaks found
[main da560c4] Check gitleaks
 1 file changed, 1 insertion(+), 1 deletion(-)
```

## Middle 

Clone this repo and create pre-commit for gitleaks
```
git clone <repo_url>
cp <repo_dir>/pre-commit-examples/pre-commit-middle .git/hooks/pre-commit
chmod +x .git/hooks/pre-commit
```
Now you can commit your code as usual and use advantages of the gitleaks.
If gitleaks is not present on the system, it will be automatically installed based on the operating system.

## Senior
