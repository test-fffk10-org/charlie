# Charlie - Express Application

A simple Express.js application skeleton with modern libraries and best practices.

## Installation

```bash
npm install
```

Copy the example environment file and configure your settings:

```bash
cp .env.example .env
```

Edit `.env` to set your database connection string and other environment variables.

## Usage

Start the server:

```bash
npm start
```

The server will run on port 3000 by default. You can set a custom port using the PORT environment variable:

```bash
PORT=8080 npm start
```

## API Endpoints

- `GET /` - Welcome message
- `GET /health` - Health check endpoint

## Development

Run the application in development mode:

```bash
npm run dev
```

## Libraries Used

This application includes the following libraries:

- **Express** (v5.1.0) - Fast, unopinionated, minimalist web framework
- **Prisma** (v6.1.0) - Next-generation ORM for Node.js and TypeScript
- **dotenv** (v16.4.5) - Environment variable management
- **cors** (v2.8.5) - CORS middleware for Express
- **helmet** (v8.0.0) - Security headers middleware
- **morgan** (v1.10.0) - HTTP request logger

## Database with Prisma

This project uses Prisma as the ORM. To get started with the database:

1. Configure your `DATABASE_URL` in the `.env` file
2. Define your data models in `prisma/schema.prisma`
3. Run migrations:
   ```bash
   npx prisma migrate dev --name init
   ```
4. Generate Prisma Client:
   ```bash
   npx prisma generate
   ```

For more information, see the [Prisma documentation](https://www.prisma.io/docs/).
