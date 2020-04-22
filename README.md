# Mongo DB Cookbok :computer: :cd: :electric_plug:

This project consists of a mongodb Cookbook. The Cookbook installs mongodb from the source.

### Prerequisites
- In order to run the Mongodb Cookbook you must ensure you have the packages bellow:

```python
- git
- chef
- Virtualbox
- Vagrant
- AWS CLI v2
```
### What is Chef?

- A company released in 2009 which created a tool that goes after its name `Chef`. This tool was designed as a configuration management written in ruby.
- Chef helps by managing the infrastructure of code to create an autonomous process. Chef has a client server architecture meaning it is able to support various platforms such as; Ubuntu, Windows, OS x, Solaris, etc.

### Installation
- In order to download this repository, open your terminal and `mkdir <filename>`, then `cd` into that new directory and run:

```python
git clone git@github.com:Aymz96/MongoCookbookStarterCode.git
```

### Run Cookbook tests
- In order to test the Mongodb Cookbook, you must first navigate into the Cookbook through the terminal, then execute the steps below:

### Testing Cookbook
- Once in the directory you will be testing both the ChefSpec and ChefInspec.

**ChefSpec**
run:
```python
chef exec rspec
```
- This tests for what has been inputted within the default_spec.rb
- This can be found within the `spec/unit` directory.

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

☆彡(ノ^ ^)ノ Congratulations ヘ(^ ^ヘ)☆彡
:v::ok_hand:
