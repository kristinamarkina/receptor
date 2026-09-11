FROM quay.io/ansible/receptor:latest

RUN set -x \
    # Set fastest repo
    echo 'fastestmirror=1' >> /etc/dnf/dnf.conf \
    # Add debug tools
    && yum install -y iputils nano htop vim \
    && yum clean all \
    && rm -rf /var/cache/yum
