FROM lwieske/java-8
WORKDIR /usr
ADD startup.sh /usr/startup.sh

# For Openshift
RUN chown -R 1001:0 /usr && \
    chmod -R ug+rwX /usr
USER 1001

ENTRYPOINT ["sh","./startup.sh"]
