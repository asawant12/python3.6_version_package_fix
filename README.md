# python3.6_version_package_fix
in python 3.6.5 pip install was failing for version. I have fixed it here. Please clone download and install

Here is the issue

myvenv) trial #$ pip --version

pip 10.0.1 from /Users/amit.sawant/.virtualenvs/myvenv/lib/python3.6/site-packages/pip (python 3.6)

(myvenv) trial #$ pip install version

Collecting version

  Using cached https://files.pythonhosted.org/packages/fd/b6/fa3b2c859d4d8817a106e4272029d78a2afbca0a27139997a4e5515bbf60/version-0.1.1.tar.gz

    Complete output from command python setup.py egg_info:

    Traceback (most recent call last):

      File "<string>", line 1, in <module>

      File "/private/var/folders/44/0b94tr3s683c67gqgxgfp7mc0000gp/T/pip-install-hbbewl3s/version/setup.py", line 4, in <module>

        from version import __version__

      File "/private/var/folders/44/0b94tr3s683c67gqgxgfp7mc0000gp/T/pip-install-hbbewl3s/version/version.py", line 2, in <module>

        from itertools import izip_longest

    ImportError: cannot import name 'izip_longest'

    

    ----------------------------------------

Command "python setup.py egg_info" failed with error code 1 in /private/var/folders/44/0b94tr3s683c67gqgxgfp7mc0000gp/T/pip-install-hbbewl3s/version/

(myvenv) trial #$ 
