FROM ghcr.io/drpayyne/chrome-puppeteer

USER root

WORKDIR /var/www/html
COPY generate.sh /usr/bin/generate
COPY bundle.sh /usr/bin/bundle

RUN npm install -g magepack@^2.3 && npm cache clean --force

CMD tail -f /dev/null

USER chrome
