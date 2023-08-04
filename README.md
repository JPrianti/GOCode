### Go example to create docker image, deploy it locally and use Delve for remote debugging
- Commands used:
    - Web page address:  http://127.0.0.1:5000   (Stop sever using "ctrl c" on terminal)
    - Docker command: docker build --tag godebug .
    - Docker command to lauch container: Docker run --security-opt="seccomp=unconfined" --cap-add=SYS_PTRACE -p:5001:5000 -p:2345:2345 godebug

