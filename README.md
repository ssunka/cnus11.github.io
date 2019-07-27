## How Our Restaurant ChatBot Sends Mail
We use a snmpd daemon which comes with python installation for sending
mails. 'aiosmtpd' provides a main entry point which can be used to
run the server on the command line.

There are 2 ways to run the server either by passing it to Python directly
or the entry point may also be installed as the aiosmtpd command,
##### $ `python3 -m aiosmtpd -n`
##### $ `aiosmtpd -n`

This starts a server on localhost, port 8025 without setting the uid to
‘nobody’ (i.e. because you aren’t running it as root)

---
### How to install `aiosnmpd`?
>$pip install [aiosnmp](https://pypi.org/project/aiosnmp/)

---
### Sample Mail Response
![sample](https://github.com/mr-samarjit-adhikari/image-repo/blob/master/Screenshot%20from%202019-07-26%2000-25-08.png?raw=true)

---
[Click for more information](https://aiosmtpd.readthedocs.io/en/latest/aiosmtpd/docs/cli.html)

### Rasa versions used for testing
rasa-core==0.8.2
rasa-nlu==0.11.5
rasa-sdk==1.1.0
rasa-x==0.19.5

### Rasa Output
Sample use cases have been executed for reference in output.txt file.
