FROM node:18-alpine

# Creating group and user
# RUN addgroup --system --gid 1001 appgroup && adduser --system --uid 1001 --ingroup appgroup appuser

# USER appuser

WORKDIR /app
# RUN npm install -g yarn
COPY . .
RUN yarn


# CMD ["tail", "-f", "/dev/null"]
CMD ["yarn", "dev"]