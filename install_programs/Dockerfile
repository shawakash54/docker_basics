FROM debian:sid
# -y flag is for stating always yes
RUN apt-get -y update
RUN apt-get install nano
# The following way of writing a command is know as exec. form
# when the command runs, run the command /bin/nano with the argument /tmp/notes
CMD ["bin/nano", "/tmp/notes"]