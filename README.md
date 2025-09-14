# MEDILINK Healthcare Platform

MEDILINK is a SaaS platform that digitizes hospital workflows by enabling doctors to create digital prescriptions, lab reports, and discharge summaries with digital signatures. The platform integrates with ABHA/ABDM for national-level health record storage.

## Features

- Digital prescriptions with QR codes
- Lab reports and discharge summaries
- Digital signatures for medical records
- ABDM/ABHA integration
- Pharmacy verification system
- Secure document storage

## Prerequisites

- Node.js v14+
- MongoDB v4.4+
- AWS Account (for S3 storage)
- ABDM API credentials

## Installation

1. Clone the repository
2. Install dependencies:
   ```
   npm install
   ```
3. Create a `.env` file with required environment variables (see `.env.example`)
4. Start the server:
   ```
   npm run dev
   ```

## Environment Variables

Create a `.env` file with the following variables:

```
PORT=3000
MONGODB_URI=mongodb://localhost:27017/medilink
JWT_SECRET=your_jwt_secret
AWS_ACCESS_KEY_ID=your_aws_access_key
AWS_SECRET_ACCESS_KEY=your_aws_secret_key
AWS_BUCKET_NAME=your_bucket_name
ABDM_API_KEY=your_abdm_api_key
```

## Project Structure

```
medilink/
├── src/
│   ├── config/        # Configuration files
│   ├── controllers/   # Request handlers
│   ├── models/       # Database models
│   ├── routes/       # API routes
│   ├── middleware/   # Custom middleware
│   ├── utils/        # Utility functions
│   └── server.js     # Entry point
├── public/           # Static files
└── tests/           # Test files
```

## API Documentation

See [API.md](./API.md) for detailed API documentation.

## License

MIT