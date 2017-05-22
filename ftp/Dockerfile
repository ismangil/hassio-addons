FROM %%BASE_IMAGE%%

ENV VERSION %%VERSION%%
ENV LANG C.UTF-8

# Copy data for add-on
COPY run.sh /

# Install requirements for add-on
RUN apk add --no-cache jq vsftpd 

RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
