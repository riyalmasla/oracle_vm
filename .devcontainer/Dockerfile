# Use the specified Oracle 19c image as the base
FROM doctorkirk/oracle-19c

# Set the container name
LABEL name="oracle-19c"

# Expose the port for Oracle database
EXPOSE 1521

# Set environment variables
ENV ORACLE_SID=orcl
ENV ORACLE_PWD=horlicks
ENV ORACLE_HOME=/opt/oracle/product/19c/dbhome_1/
ENV ORACLE_BASE=/opt/oracle/
ENV PATH="$PATH:/opt/oracle/product/19c/dbhome_1/:/opt/oracle/product/19c/dbhome_1/bin/:%ORACLE_BASE:/opt/oracle/product/19c/dbhome_1/OPatch/"
# ADD /opt/oracle/product/19c/dbhome_1/bin/ to path

# ENV ORACLE_CHARACTERSET=[CHARSET]

VOLUME /opt/oracle/oradata

# [Optional] Uncomment this section to install additional OS packages.
# RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
#     && apt-get -y install --no-install-recommends <your-package-list-here>