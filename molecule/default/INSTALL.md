# Installing the local testing env

Install [virtualbox](https://www.virtualbox.org/) (currently using version 6.1.22 r144080)

Install [vagrant](https://www.vagrantup.com/) (currently using version 2.2.16)

Create a python virtual env.

Install the dependencies listed in the requirements.txt at the root directory of this project :
```
pip install -r requirements.txt
```

# Running tests with the local environement

This project uses the [molecule](https://molecule.readthedocs.io/en/latest/) testing framework with the vagrant plugin alongside the virtualbox provider to create a testing plateform, deploy to it and then destroy it.

To run the full testing suite run the following command after activating your python virtualenv:
```
molecule test
```

For more informations on other usable commands, check the [molecule CLI documentation](https://molecule.readthedocs.io/en/latest/getting-started.html#run-test-sequence-commands).