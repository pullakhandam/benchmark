Put your benchmarks in the results repository.

IF A BENCHMARK DOES NOT WORK OR FAILS, PLEASE FIX IT.
ENGAGE IN DISCUSSION ON PIAZZA.

File naming conventions should match the following:

USERNAME is your unique username

```
pip install cloudmesh-installer -U
cloudmesh-installer git clone cloud
cloudmesh-installer install cloud

cms set cloud=AWS
cms debug on

cms init
cms key add 
cms key upload --cloud=AWS

cms vm boot # making sure that machine can boot
cms vm list --refresh  # making sure that can write to mongo
```

## Local, Security, and Cloud Tests

- 1_local-USERNAME.txt
- 2_local-USERNAME.txt
- 2_security-USERNAME.txt
- cloud-aws-USERNAME.txt

## Others

- aws-USERNAME.txt
- azure-USERNAMEtxt
- google-USERNAME.txt

## Storage Tests

- storage-USERNAME.txt

## Notes

- other storage tests are in cloudmesh-storage\tests

## How to create the output

let us assume you like to execute all tests in teh directory: 

    1_local

Then you use the command

    pytest -v --capture=no  tests/1_local > 1_local-USERNAME.txt

or 

    pytest -v --capture=no  tests/1_local | tee 1_local-USERNAME.txt


  

You only have to execute the local tests once as the cloud providers ar
irrelevant for them, e.g. the cloud is "local"


## Tests

    pytest -v --capture=no  tests/1_local | tee 1_local-USERNAME.txt
    pytest -v --capture=no  tests/2_local | tee 2_local-USERNAME.txt
    pytest -v --capture=no  tests/2_security | tee 2_security-USERNAME.txt
    pytest -v --capture=no  tests/cloud | tee cloud-USERNAME.txt
