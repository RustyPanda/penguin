FROM node:8

WORKDIR /app
RUN echo
COPY * ./

RUN npm install

ENV appSecret = 9c63803061c6057e9e0f208a5c6169c8
ENV pageAccessToken = EAAIUXWu4OXMBAEaowiV9XZAQNkuBJDniFJZCY39XrOZCdhNbG7L3bsCZCZAQS338OvLUyh49HcMpJ9hIBIlXXlOJQD6cdkJpDUjnRmUEAqPdmfKTO7YiaCFMMsBQKdD47mf7ocvgV6yhBlSZB1RPZBVrY1NnrJCWNxpDPlvPAGBacyvhSjX8CWG
ENV validationToken = TOKEN
ENV serverURL = to_be_set_manually

RUN ls /app/config
CMD node app.js