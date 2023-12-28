FROM ubuntu:latest

# Install necessary packages
RUN apt-get update && apt-get install -y samba krb5-user winbind

# Copy the Samba configuration file
COPY smb.conf /etc/samba/smb.conf

# Expose the necessary ports
EXPOSE 137/udp 138/udp 139 445

# Start the Samba service
CMD ["smbd", "--foreground", "--no-process-group"]
