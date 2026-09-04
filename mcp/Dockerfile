FROM node:20-slim
WORKDIR /app
COPY mcp/package.json mcp/pnpm-lock.yaml ./
RUN npm install -g pnpm && pnpm install --frozen-lockfile
COPY mcp/ .
EXPOSE 8787
CMD ["node", "server.js"]

