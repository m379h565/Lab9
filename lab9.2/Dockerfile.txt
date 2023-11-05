# Set the base image to use
FROM gcc:latest
# Copy the C program into the container
COPY Lab5Part2.c .
# Compile the C program
RUN gcc -o Lab5Part2 Lab5Part2.c
# Set the command to run when the container starts
CMD ["./Lab5Part2"]