Put your benchmarks in the results repository.

IF A BENCHMARK DOES NOT WORK OR FAILS, PLEASE FIX IT.
ENGAGE IN DISCUSSION ON PIAZZA.

File naming conventions should match the following:

USERNAME is your unique username

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

Then you use the command, 

pytest -v --capture=no  tests/1_local > 1_local-USERNAME.txt

YOu only have to execute the local tests once