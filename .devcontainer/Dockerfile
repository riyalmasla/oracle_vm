# Use the specified Oracle 19c image as the base
FROM doctorkirk/oracle-19c

# Set the container name
LABEL name="oracle-19c"

# Expose the port for Oracle database
EXPOSE 1521

# Set environment variables
ENV ORACLE_SID="system"
ENV ORACLE_PWD="horlicks"
# ENV ORACLE_CHARACTERSET=[CHARSET]

# [Optional] Uncomment this section to install additional OS packages.
# RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
#     && apt-get -y install --no-install-recommends <your-package-list-here>
