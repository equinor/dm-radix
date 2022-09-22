FROM datamodelingtool.azurecr.io/dmt/web

ARG AUTH_ENABLED=0
ARG REDIRECT_URI=http://localhost/

ENV REACT_APP_AUTH_REDIRECT_URI=$REDIRECT_URI
ENV REACT_APP_AUTH=$AUTH_ENABLED

ENV REACT_APP_AUTH_SCOPE=api://97a6b5bd-63fb-42c6-bb75-7e5de2394ba0/dmss
ENV REACT_APP_AUTH_CLIENT_ID=97a6b5bd-63fb-42c6-bb75-7e5de2394ba0
ENV REACT_APP_TOKEN_ENDPOINT=https://login.microsoftonline.com/3aa4a235-b6e2-48d5-9195-7fcf05b459b0/oauth2/v2.0/token
ENV REACT_APP_AUTH_ENDPOINT=https://login.microsoftonline.com/3aa4a235-b6e2-48d5-9195-7fcf05b459b0/oauth2/v2.0/authorize
ENV REACT_APP_LOGOUT_ENDPOINT=https://login.microsoftonline.com/3aa4a235-b6e2-48d5-9195-7fcf05b459b0/oauth2/logout
