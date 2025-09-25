# 🏡 RealEstate - MERN Stack Property Platform

A full-stack real estate platform built with the MERN stack (MongoDB, Express.js, React, Node.js), providing comprehensive property management and listing services.

## ✨ Features

### 🔍 Property Search & Discovery
- **Advanced Search**: Filter properties by location, price range, type, and amenities
- **Interactive Maps**: View property locations with integrated mapping
- **Property Listings**: Detailed property information with high-quality images
- **Favorites**: Save and manage favorite properties
- **Property Comparison**: Compare multiple properties side-by-side

### 👥 User Management
- **User Authentication**: Secure registration and login system
- **User Profiles**: Personalized dashboards for buyers, sellers, and agents
- **Role-based Access**: Different permissions for different user types
- **Profile Management**: Update personal information and preferences

### 🏠 Property Management
- **Property Listings**: Create, edit, and manage property listings
- **Image Uploads**: Multiple image support with gallery functionality
- **Property Details**: Comprehensive property information forms
- **Listing Status**: Track property availability and status
- **Agent Tools**: Professional tools for real estate agents

### 💬 Communication
- **Contact Forms**: Direct communication between buyers and sellers
- **Inquiry Management**: Track and manage property inquiries
- **Messaging System**: In-app messaging for users
- **Notifications**: Real-time updates on property activities

## 🛠️ Tech Stack

### Frontend
- **React.js** - Component-based UI library
- **React Router** - Client-side routing
- **Axios** - HTTP client for API requests
- **CSS3/SCSS** - Styling and responsive design
- **React Hooks** - Modern React state management

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB object modeling
- **JWT** - JSON Web Tokens for authentication
- **bcryptjs** - Password hashing

### Additional Tools
- **Multer** - File upload handling
- **Cloudinary/AWS S3** - Image storage and optimization
- **Nodemailer** - Email notifications
- **CORS** - Cross-origin resource sharing
- **dotenv** - Environment variable management

## 🚀 Getting Started

### Prerequisites
- Node.js (version 14 or later)
- npm or yarn package manager
- MongoDB database (local or cloud)
- Cloudinary account (for image uploads)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/HRISHIKESH-hackoff/RealEstate.git
   cd RealEstate
   ```

2. **Install dependencies**
   
   Backend dependencies:
   ```bash
   cd api
   npm install
   ```
   
   Frontend dependencies:
   ```bash
   cd ../client
   npm install
   ```

3. **Environment Variables**
   
   Create `.env` file in the `api` directory:
   ```env
   MONGODB_URI=mongodb://localhost:27017/realestate
   JWT_SECRET=your_jwt_secret_key
   JWT_EXPIRES_IN=7d
   
   # Cloudinary Config (Optional)
   CLOUDINARY_CLOUD_NAME=your_cloud_name
   CLOUDINARY_API_KEY=your_api_key
   CLOUDINARY_API_SECRET=your_api_secret
   
   # Email Config (Optional)
   EMAIL_HOST=smtp.gmail.com
   EMAIL_PORT=587
   EMAIL_USER=your_email@gmail.com
   EMAIL_PASS=your_app_password
   
   # App Config
   NODE_ENV=development
   PORT=5000
   CLIENT_URL=http://localhost:3000
   ```

4. **Start the application**
   
   Start backend server:
   ```bash
   cd api
   npm start
   # or for development
   npm run dev
   ```
   
   Start frontend (in a new terminal):
   ```bash
   cd client
   npm start
   ```

5. **Access the application**
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:5000

## 📁 Project Structure

```
RealEstate/
├── api/                    # Backend server
│   ├── controllers/        # Route controllers
│   ├── models/            # Database models
│   ├── routes/            # API routes
│   ├── middleware/        # Custom middleware
│   ├── utils/             # Utility functions
│   ├── config/            # Configuration files
│   └── server.js          # Main server file
│
├── client/                # Frontend React app
│   ├── public/           # Public assets
│   ├── src/              # Source code
│   │   ├── components/   # React components
│   │   ├── pages/        # Page components
│   │   ├── hooks/        # Custom hooks
│   │   ├── context/      # React context
│   │   ├── services/     # API services
│   │   ├── utils/        # Utility functions
│   │   └── styles/       # CSS/SCSS files
│   └── package.json      # Frontend dependencies
│
├── .gitignore            # Git ignore rules
├── package.json          # Root dependencies
└── README.md             # Project documentation
```

## 🔧 API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout
- `GET /api/auth/me` - Get current user

### Properties
- `GET /api/properties` - Get all properties
- `GET /api/properties/:id` - Get single property
- `POST /api/properties` - Create new property
- `PUT /api/properties/:id` - Update property
- `DELETE /api/properties/:id` - Delete property
- `GET /api/properties/search` - Search properties

### Users
- `GET /api/users/profile` - Get user profile
- `PUT /api/users/profile` - Update user profile
- `POST /api/users/favorites/:id` - Add to favorites
- `DELETE /api/users/favorites/:id` - Remove from favorites

### Contact & Inquiries
- `POST /api/contact` - Send contact message
- `POST /api/inquiries` - Send property inquiry
- `GET /api/inquiries` - Get user inquiries

## 🎯 Usage

### For Property Buyers
1. **Browse Properties**: Search and filter available properties
2. **View Details**: Check comprehensive property information
3. **Save Favorites**: Create a wishlist of interested properties
4. **Contact Agents**: Reach out to property agents directly
5. **Schedule Visits**: Arrange property viewings

### For Property Sellers/Agents
1. **Create Listings**: Add new properties with detailed information
2. **Manage Properties**: Update, edit, or remove existing listings
3. **Track Inquiries**: Monitor and respond to buyer inquiries
4. **Analytics**: View property performance and engagement
5. **Profile Management**: Maintain professional agent profiles

## 🌟 Features in Development
- [ ] Advanced property analytics and insights
- [ ] Mortgage calculator integration
- [ ] Virtual property tours
- [ ] Real-time chat system
- [ ] Mobile app development
- [ ] Multi-language support
- [ ] Property price predictions
- [ ] Integration with MLS systems

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Hrishikesh Mandal**
- GitHub: [@HRISHIKESH-hackoff](https://github.com/HRISHIKESH-hackoff)
- Email: hrishikesh@example.com

## 🙏 Acknowledgments

- [MongoDB](https://www.mongodb.com/) for the flexible NoSQL database
- [Express.js](https://expressjs.com/) for the robust web framework
- [React](https://reactjs.org/) for the powerful frontend library
- [Node.js](https://nodejs.org/) for the JavaScript runtime
- [Cloudinary](https://cloudinary.com/) for image management services

⭐ If you found this project helpful, please give it a star on GitHub!

Happy Coding! 🏡✨
