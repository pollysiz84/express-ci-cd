FROM node:16
WORKDIR /app
COPY . .
ENV REACT_APP_BACKEND_URL=http://localhost/api
RUN npm install
RUN npm run build
RUN npm install -g serve
EXPOSE 5000
CMD ["serve", "-s", "build", "-l", "5000"]
