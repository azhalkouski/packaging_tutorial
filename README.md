# packaging_tutorial


# Packaging Python Projects
https://packaging.python.org/en/latest/tutorials/packaging-projects/


 # build
  Run `python3 -m build` and it'll produce two builds under dist/ directory
  dist/
    - example_package_azhalkouski-0.0.1-py3-none-any.whl
    - example_package_azhalkouski-0.0.1.tar.gz

# test run
  If you want to test run the package do the following
  1. download the wheel archive (it's not stored in PyPI) OR BUILD IT YOURSELF
  2. mkdir test_run_dir && python3 -m venv env && source env/bin/activate
  3. pip install path_to_your_downloaded_wheel archive - that is going to install
  the package under site-packages in your virtual env. specifically in 
  `test_run_dir/env/lib/python3.xx/site-packages/example_package_azhalkouski`
  4. python3 -m example_package_azhalkouski which should print `True` in your terminal