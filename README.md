# LaTeX Diff Tutorial
## This tutorial is for course - English for Science and Technology, NTHU CS.
### Environment Setup
#### 1. Code clone
```bash
git clone https://est-latex.sjf.tw/shared/LaTeX_Diff_Tutorial
cd LaTeX_Diff_Tutorial/
```
#### 2. Run init script
```bash
./0_init.sh
```
```yaml
Enter user name for git:
Enter user email for git:
Reset (origin) remote? [Y/n]    # default Y. prees Enter to continue; type N if no need
- Enter remote url:
- Add secondary push remote? [y/N]    # default N, add if needed
-  Enter secondary remote url:

Install TexLive-Science (SW distribution for TeX)? [Y/n]
Install Latexdiff (To generate diff PDFs)? [Y/n]
Install Texmaker (Open-source LaTeX editor)? [Y/n]
Install pip3 (The Python Package Installer)? [y/N]    # install if needed 
Install Pipenv (Virtual environment for Python)? [y/N]    # install if needed
Init pipenv (For gen_diff.py)? [Y/n]
```
### Generate Paper PDF
```bash
# Prerequisite: TexLive-Science
# Target dir: build/Paper.pdf
./1_gen_paper.sh
```
### Generate Diff PDFs
```bash
# Prerequisite: python3, pip3, pipenv, and gitpython
# Target dir: diff/([1-9][0-9]*-USR-COMMIT_MSG.pdf)*
./2_gen_diff.sh
```