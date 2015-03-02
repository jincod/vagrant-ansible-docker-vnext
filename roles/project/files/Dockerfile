FROM microsoft/aspnet

COPY ./app /root/app
WORKDIR /root/app
RUN ["kpm", "restore"]

EXPOSE 5004
CMD []
ENTRYPOINT ["k", "kestrel"]