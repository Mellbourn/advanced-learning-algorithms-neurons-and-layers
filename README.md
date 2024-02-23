# How to set up a new Python environment properly

1. `mkdir my-project`
2. `cd my-project`
3. `cp /Users/klas.mellbourn/code/private/ai/coursera/supervised-machine-learning/.gitignore .`
4. **<code>python -m venv .venv</code></strong>
5. <code>cp /Users/klas.mellbourn/code/private/ai/coursera/supervised-machine-learning/supervised-machine-learning/.envrc .</code>
6. <code>cat .envrc</code>
    1. <code>export VIRTUAL_ENV=.venv</code>
    2. <code>layout python</code>
7. <code>direnv allow</code>
8. <code>git init</code>
9. <code>git commit -m "initial commit of python project"</code>
10. Create or copy the code or notebook
11. <code>g add .</code>
12. <code>g commit -m "added Jupyter Notebook files"</code>
13. <code>gh repo create --public --push --source .</code>
14. <code>code .</code>
15. <code>&lt;open a Jupyter Notebook></code>
16. <code>Shift-enter</code>
17. <code>&lt;Choose python environment></code>
18. <code>&lt;choose .venv, which is recommended></code>
19. When asked <code>"Running cellcodes with '.venv' requires the ipykernel package"</code>
    3. Choose <code>"Install"</code>
20. If further packages are needed by python, (e.g. you get ModuleNotFoundError dependency errors when running jupyter cells)
    4. Open a terminal
    5. <code>pip install &lt;package></code>
    6. e.g.
    7. <code>pip install numpy matplotlib ipywidgets</code>
21. If you need tensorflow, follow [https://www.tensorflow.org/install](https://www.tensorflow.org/install)
    8. <code>asdf install python 3.11.8</code>
    9. <code>asdf local python 3.11.8</code>
    10. <code>cd &lt;into directory></code>
    11. <code>python -m venv .venv</code>
    12. <code>python -m pip install --upgrade https://files.pythonhosted.org/packages/85/15/cf99a373812d37f8ae99752a34a9f5f690d820ceb5b302e922705bc18944/tensorflow-2.15.0-cp311-cp311-macosx_12_0_arm64.whl</code>

duplicated from [Klas Google Docs document](https://docs.google.com/document/d/1P3bhtnPcODSnqDpTFKYxM2qKpuhbgixnh53RUwVF580/edit)
