# 🍽️ Feed The Need

<div align="center">

![Feed The Need Logo](https://user-images.githubusercontent.com/113793678/205454471-648128b3-0a64-40ce-bce1-bd555b718cdc.png)

*Bridging the gap between food excess and food scarcity*

[![Made with Love](https://img.shields.io/badge/Made%20with-Love-red.svg)](https://github.com/Cipher-unhsiV/Feed-The-Need)

</div>

## 📋 About The Project

**The Challenge**: Every year, while **573 million people** face starvation, food that could feed **565 million people** goes to waste. This stark contrast highlights a critical distribution problem in our food system.

**Our Solution**: Feed The Need is an innovative platform that connects three key stakeholders:
- 🙋‍♂️ Food Seekers (individuals facing food insecurity)
- 🤲 Food Donors (those with excess food)
- 🏢 NGOs & Social Activists (facilitators)

## 👥 Key Roles

1. **General Public** 
   - Acts as our eyes on the ground
   - Reports food seekers through the portal
   - Provides location and demographic information

2. **Food Donors**
   - Individuals or organizations with excess food
   - Register available food quantities and location
   - Coordinate with NGOs for collection

3. **NGO Partners**
   - Bridge between donors and seekers
   - Handle food collection and distribution
   - Ensure food safety and proper delivery

4. **Super-admin**
   - System oversight and management
   - Access to all platform features
   - Data analysis and reporting

## 🎯 How It Works

![Dashboard Preview](https://user-images.githubusercontent.com/113793678/205455521-1969da2c-2c8a-497a-8287-edd3302f15d3.png)

### Process Flow:

1. **Identification** 📍
   - General public reports food seekers
   - Location tracking
   - Optional contact information
   
2. **Donation Registration** 📝
   - Donors input food availability
   - Specify serving capacity
   - Share location details

3. **Distribution** 🚚
   - NGOs view active donors and seekers
   - Coordinate food collection
   - Manage delivery logistics

## 🛠️ Technology Stack

### Frontend
- HTML5
- CSS3
- JavaScript
- EJS (Embedded JavaScript templates)

### Backend
- Node.js
- Express.js

#### API Endpoints

**Authentication**
```bash
POST /register         # Register new user (NGO or Donor)
POST /login           # User login with passport authentication
GET  /logout          # User logout and session termination
```

**Donor Operations**
```bash
GET  /donarform       # Render donor food submission form
POST /donarform       # Create new food donation entry
GET  /donarpage       # Display donor dashboard with history
GET  /editdonardetails # Render donor profile edit form
PUT  /editdonardetails # Update donor profile information
```

**NGO Operations**
```bash
GET  /ngodashboard     # Display NGO dashboard
GET  /editngodetails   # Render NGO profile edit form
PUT  /editngodetails   # Update NGO profile information
GET  /provideservice   # List available donations and requests
POST /provideService   # Create donor-receiver matches
```

**Public Access**
```bash
GET  /publicform      # Render food seeker report form
POST /publicform      # Submit new food seeker information
```

**Super Admin Routes**
```bash
GET  /superadmin/dashboard   # Display admin control panel
GET  /superadmin/lod         # Show registered donors list
GET  /superadmin/listofngo   # Show registered NGOs list
GET  /superadmin/donorlog    # View donor activity logs
GET  /superadmin/ngolog      # View NGO activity logs
GET  /superadmin/publiclog   # View public reports log
```

**Base Routes**
```bash
GET  /                # Render main dashboard
GET  /register        # Display registration page
GET  /login           # Display login page
```

### Database
- MongoDB
  - Users Collection
  - Donations Collection
  - History Collection
  - Logs Collection

### Development Tools
- Python (for data processing)
- Markdown (for documentation)

## 👨‍💻 Development Team

<div align="center">

| Vishnuvasan | Rahul | John |
|-------------|-------|------|
| [![Vishnuvasan](https://avatars.githubusercontent.com/Cipher-unhsiV?s=150&v=1)](https://github.com/Cipher-unhsiV) | [![Rahul](https://avatars.githubusercontent.com/Rahul040202?s=150&v=1)](https://github.com/Rahul040202) | [![John](https://avatars.githubusercontent.com/john-williams-m?s=150&v=1)](https://github.com/john-williams-m) |
| [GitHub](https://github.com/Cipher-unhsiV) | [GitHub](https://github.com/Rahul040202) | [GitHub](https://github.com/john-williams-m) |
| [LinkedIn](https://www.linkedin.com/in/cipher-unhsiv/) | [LinkedIn](https://www.linkedin.com/in/rahul-g-9ba993224/) | [LinkedIn](https://www.linkedin.com/in/john-williams-m) |

</div>

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/feed-the-need.git
   ```

2. **Install dependencies**
   ```bash
   cd feed-the-need
   npm install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env
   # Edit .env with your MongoDB URI and other configurations
   ```

4. **Run the application**
   ```bash
   npm start
   ```

## 🤝 Contributing

We welcome contributions from the community! If you'd like to contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📬 Contact

For questions or suggestions, please reach out to any team member through their LinkedIn profiles.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
