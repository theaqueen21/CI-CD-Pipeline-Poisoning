# Spilling A GitHub Repository's Secrets Using GitLeaks

Disclaimer: The GitHub Repository Used As An Example Was Part Of A CTF Challenge And No Real Secrets Or Credentials Are Shown.

Disclaimer: This Is Merely For Educational Purposes Or For Solving CTFs And Should Not Be Attempted Without The User's Permission Or Consent.

>Note: Secrets Include Credentials, API Tokens, RSA Certificates etc...

0. Clone The Target Repository

```
git clone {Repository.git}
```

1. Install GitLeaks Using apt

```
sudo apt-get install gitleaks -y
```

![1](https://github.com/theaqueen21/CI-CD-Pipeline-Poisoning/assets/94680549/573ded0c-00b5-4055-9114-4a9d20dc9449)

2. Run The Command Below In The Cloned Repository Folder

```
gitleaks detect
``` 
GitLeaks Automatically Looks For Leaks Or So Called Secrets In The Logs, Commits, And Files Of The Repository

![2](https://github.com/theaqueen21/CI-CD-Pipeline-Poisoning/assets/94680549/91a4672c-6e45-4edb-8fdf-603e87270594)

![3](https://github.com/theaqueen21/CI-CD-Pipeline-Poisoning/assets/94680549/e4251de6-d398-46e8-9935-b967440c1770)

3. If Leaks Are Found, Run The Command Below To Display The Leaks Or So Called Secrets

```
gitleaks detect -v
```

![4](https://github.com/theaqueen21/CI-CD-Pipeline-Poisoning/assets/94680549/54aa5647-5f21-4316-b209-d41dc997c4ab)

As You Can See A PyPi API Token Was Found In This Attempt Along With Other Secrets

![5](https://github.com/theaqueen21/CI-CD-Pipeline-Poisoning/assets/94680549/553c2279-d0e7-45f0-8787-b32858815e89)

![6](https://github.com/theaqueen21/CI-CD-Pipeline-Poisoning/assets/94680549/caa15ffc-d033-4291-ac6a-75e7fff0c60a)

![7](https://github.com/theaqueen21/CI-CD-Pipeline-Poisoning/assets/94680549/eab75430-a87a-4f9a-a7e1-238d335b0b90)

