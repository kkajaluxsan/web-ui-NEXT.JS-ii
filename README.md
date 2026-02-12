# Service Provider Management Application

A modern Next.js 14 application for managing service providers with interactive maps, dynamic forms, and a professional UI design.

## Features

- **Next.js 14 with App Router** - Latest React framework with server and client components
- **Interactive Maps** - React Leaflet integration for location selection
- **Responsive Design** - Tailwind CSS for styling
- **Dynamic Forms** - Multiple form sections with real-time state management
- **Tab Navigation** - Switch between different form sections seamlessly
- **Professional UI** - Dark navy headers, rounded inputs, and consistent spacing

## Tech Stack

- **Next.js 14** - React framework
- **TypeScript** - Type safety
- **Tailwind CSS** - Utility-first CSS framework
- **React Leaflet** - Interactive mapping
- **Leaflet** - Mapping library
- **Lucide React** - Icon library

## Installation

1. Clone the repository or navigate to the project directory:
```bash
cd web_ui
```

2. Install dependencies:
```bash
npm install
```

3. Run the development server:
```bash
npm run dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

## Project Structure

```
src/
├── app/
│   ├── layout.tsx       # Root layout component
│   ├── page.tsx         # Main page with state management
│   └── globals.css      # Global styles
├── components/
│   ├── layout/
│   │   ├── Sidebar.tsx  # Navigation sidebar
│   │   └── Header.tsx   # Top header with breadcrumb
│   ├── tabs/
│   │   └── Tabs.tsx     # Tab navigation component
│   ├── forms/
│   │   ├── MainDetails.tsx  # Main details form
│   │   └── SubDetails.tsx   # Sub details form
│   ├── map/
│   │   └── MapComponent.tsx # Interactive map component
│   └── ui/
│       ├── Input.tsx    # Input field component
│       └── Select.tsx   # Select dropdown component
├── config files (tailwind.config.ts, tsconfig.json, etc.)
```

## Usage

### Main Features

1. **Sidebar Navigation** - Navigate through different menu items
2. **Tab Management** - Switch between "T 01", "T 02", etc. tabs
3. **Form Submission** - Fill out Main Details and Sub Details forms
4. **Interactive Map** - Click on the map to update location coordinates
5. **Location Sync** - Latitude/Longitude inputs sync with map marker position

### Form Sections

#### Main Details
- First Name and Last Name
- Contact Person Name
- Contact Number
- Address information (District, City, Street)
- Province selection
- Interactive map for location selection
- Latitude and Longitude inputs

#### Sub Details
- Item name and type
- Total value and description
- Physical specifications (Quantity, Weight, Height, Length, Width)

## Customization

### Colors
Edit `tailwind.config.ts` to customize colors:
- `primary` - Dark navy blue (#1a3a52)
- `secondary` - Burgundy/maroon (#8B4A4A)
- `accent` - Red for required fields (#EF4444)

### Map Configuration
Edit `src/components/map/MapComponent.tsx` to:
- Change default location
- Modify map zoom level
- Add additional map features

## Building for Production

```bash
npm run build
npm start
```

## License

This project is open source and available under the MIT License.
