# Mongo DB Cookbook :computer: :cd:

This project consists of a Mongodb Cookbook. The Cookbook installs Mongodb from the source.
- This Cookbook installs Mongodb using Chef, by provisioning packages, dependancies, templates and then testing the code for functionality in the local and Virtual environment.

### Prerequisites
- In order to run the Mongodb Cookbook you must ensure you have the following below:

```CSS
- Virtualbox
- Vagrant
- AWS CLI v2
- git
- chef
    Chef Workstation:
      - ChefDK version: 4.7.73
      - Chef Infra Client version: 15.7.32
      - Chef InSpec version: 4.18.51
      - Test Kitchen version: 2.3.4
      - Foodcritic version: 16.2.0
      - Cookstyle version: 5.20.0
```
### What is Chef?

- A company released in 2009 which created a tool that goes after its name `Chef`. This tool was designed as a configuration management written in ruby.
- Chef helps by managing the infrastructure of code to create an autonomous process. Chef has a client server architecture meaning it is able to support various platforms such as; Ubuntu, Windows, OS x, Solaris, etc.

### How to install Mongodb Dev-Env
- To download this Mongodb Cookbook repository, open terminal and run the command below:

```python
git clone git@github.com:Aymz96/MongoCookbookStarterCode.git
```

### How to Run Mongodb Dev-Env tests
- To test the Mongodb Cookbook, navigate into the Cookbook through the terminal, then execute the steps below:

### How to test Mongodb Dev-Env
- Once in the directory you will be testing both the ChefSpec and ChefInspec.

**ChefSpec**
run:
```python
chef exec rspec
```
- This tests for what has been inputted within the default_spec.rb
- This can be found within the `/spec/unit` directory.

**ChefInspec**
run:
```python
Kitchen test
```
- This tests for what has been inputted within the default_test.rb
- This can be found within  the `test/integration` directory.

**ChefInspec (for the cloud)**
run:
```python
KITCHEN_YAML=.kitchen_ec2.yml kitchen test
```
- This is used to run the ChefInspec inside a cloud service. In the case of this project an EC2 machine is being used to run the tests within. The file `kitchen_ec2.yml` has been configured to run using the EC2 instance.

### Success
- Once you have run all the test as described above in the documentation. The test should all pass successfully as long as no new configurations have been done without the appropriate management.

#### Author
**Ayman Yousfi** - *Junior DevOps Engineer* - [Aymz96](https://github.com/Aymz96)
