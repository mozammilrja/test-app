# Student Progress Analytics Dashboard

A comprehensive Learning Management System (LMS) admin dashboard built with Next.js 14, TypeScript, and modern web technologies. This dashboard provides administrators with powerful analytics and insights into student performance, engagement, and progress tracking.

![Dashboard Preview](https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=800&h=400&fit=crop)

## 🚀 Features

### Dashboard Analytics

- **KPI Summary Cards**: Track key metrics including tasks assigned/completed, questions, course completion rates, time spent, and accuracy
- **Advanced Filtering**: Filter by course, date range, and performance tier
- **Student Performance Table**: Comprehensive view of all students with progress indicators
- **Interactive Charts**: Weekly progress trends visualization using Recharts
- **Student Details Modal**: Detailed analytics for individual students including milestones and progress history

### User Experience

- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Clean UI**: Minimalist design with intuitive navigation
- **Real-time Updates**: Dynamic filtering and data updates
- **Performance Indicators**: Color-coded badges for quick performance assessment
- **Smooth Animations**: Hover effects and transitions for better UX

## 🛠️ Tech Stack

- **Framework**: Next.js 14 (App Router)
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **UI Components**: ShadCN UI
- **Charts**: Recharts
- **State Management**: Zustand
- **Date Handling**: date-fns
- **Icons**: Lucide React

```

## 🚦 Getting Started

### Prerequisites

- Node.js 18+
- npm or yarn package manager

### Installation

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd student-dashboard
   ```

2. **Install dependencies**

   ```bash
   npm install
   # or
   yarn install
   ```

3. **Run the development server**

   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

### Build for Production

```bash
npm run build
npm start
```

## 📊 Dashboard Features

### KPI Cards

- **Total Tasks Assigned**: Overall tasks distributed to students
- **Tasks Completed**: Completed tasks with completion rate
- **Total Questions**: Questions assigned across all courses
- **Questions Completed**: Answered questions with accuracy metrics
- **Course Completion**: Average completion percentage
- **Time Spent**: Average study time per student
- **Active Students**: Students active in the last 7 days
- **Average Accuracy**: Overall accuracy across assessments

### Filtering System

- **Course Filter**: Filter students by specific courses
- **Performance Tier**: Filter by high/medium/low performance
- **Date Range**: Custom date range selection for enrollment periods

### Student Analytics

- **Progress Tracking**: Visual progress bars and percentages
- **Performance Badges**: Color-coded performance indicators
- **Activity Monitoring**: Last active dates and engagement metrics
- **Milestone Tracking**: Course milestone completion status

## 🎨 Design System

### Color Scheme

- **Primary**: Blue (#3B82F6) for main actions and highlights
- **Success**: Green (#10B981) for positive metrics
- **Warning**: Yellow (#F59E0B) for medium performance
- **Error**: Red (#EF4444) for low performance alerts
- **Neutral**: Gray scale for text and backgrounds

### Typography

- **Font**: Inter (Google Fonts)
- **Headings**: Bold weights for hierarchy
- **Body**: Regular weight for readability
- **Code**: Monospace for technical elements

## 🔧 Customization

### Adding New Courses

Update the courses array in `components/dashboard/filters.tsx`:

```typescript
const courses = [
  "JavaScript Fundamentals",
  "React Advanced",
  "Your New Course",
  // Add more courses
];
```

### Modifying KPI Cards

Add new KPI cards in `app/dashboard/page.tsx`:

```typescript
<KPICard
  title="Your New Metric"
  value={kpis.yourNewMetric}
  icon={YourIcon}
  trend={{ value: 5, isPositive: true }}
/>
```

### Extending Student Data

Add new fields to the Student interface in `types/student.ts`:

```typescript
export interface Student {
  // existing fields...
  yourNewField: string;
}
```

## 📱 Responsive Design

The dashboard is fully responsive with breakpoints:

- **Mobile**: < 768px (single column layout)
- **Tablet**: 768px - 1024px (2-column grid)
- **Desktop**: > 1024px (full 4-column grid)

## 🧪 Mock Data

The application uses realistic mock data generated in `lib/fake-data.ts`:

- 50 sample students with varied performance metrics
- 8 different courses across various domains
- Weekly progress data with realistic trends
- Milestone tracking with completion dates

## 🔄 State Management

Zustand store (`hooks/useStudentStore.ts`) manages:

- Student data and filtering
- Dashboard KPI calculations
- Filter state and persistence
- Selected student for modal display

## 🎯 Performance Optimization

- **Static Generation**: Next.js static export for optimal performance
- **Component Lazy Loading**: Efficient component rendering
- **Memoization**: Optimized re-renders with React hooks
- **Image Optimization**: Responsive images with proper sizing

## 🚀 Deployment

### Vercel (Recommended)

```bash
npm run build
# Deploy to Vercel
```

### Static Export

```bash
npm run build
# Serve the `out` directory
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Next.js](https://nextjs.org/) for the amazing React framework
- [ShadCN UI](https://ui.shadcn.com/) for beautiful UI components
- [Tailwind CSS](https://tailwindcss.com/) for utility-first styling
- [Recharts](https://recharts.org/) for data visualization
- [Zustand](https://github.com/pmndrs/zustand) for state management

## 📞 Support

For support, email support@example.com or create an issue in the repository.

---

**Built with ❤️ for better education management**
#   t e s t - a p p 
 
 
