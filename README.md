# Full-Stack Online Learning Platform

This project is a full-stack online learning platform inspired by Udemy, built using modern web development technologies to deliver a robust, scalable, and user-friendly experience.

---

## **Tech Stack**

1. **Frontend Framework**: Next.js 14, React, TypeScript  
2. **Database**: MySQL managed by Prisma ORM with Aiven Cloud  
3. **Authentication**: Clerk  
4. **Form Validation**: React-Hook-Form + Zod  
5. **Payment Processing**: Stripe  
6. **UI Design**: Tailwind CSS + Shadcn UI  
7. **File Uploading**: UploadThing  
8. **Video Processing and Player**: Mux  
9. **Others**: Reorder sections with drag-and-drop, progress tracking, and rich-text editing

---

## **Features Breakdown**

### **1. Server-Side & Client-Side Rendering**
- Utilize **Next.js** for seamless server-side and client-side rendering.
- Configure API routes for data fetching and leverage `getServerSideProps` or `getStaticProps` for optimized content delivery.

### **2. Database Management with Prisma ORM**
- Set up Prisma schema to define tables for users, courses, sections, purchases, and progress tracking.
- Use **Aiven Cloud** for hosting MySQL with high availability and backups.
- Perform migrations using Prisma CLI.

### **3. Create & Edit Courses with React-Hook-Form + Zod Validation**
- Build forms for instructors to create/edit courses using React-Hook-Form.
- Add validation rules using **Zod** for inputs like course title, description, category, and price.

### **4. File and Video Uploading with UploadThing**
- Integrate UploadThing to handle uploads for course images, videos, and attachments.
- Configure buckets or folders for better organization.
- Ensure support for large video files.

### **5. Reorder Sections with Drag-and-Drop**
- Use a library like `react-beautiful-dnd` to implement drag-and-drop functionality for reordering sections in a course.

### **6. API for CRUD Operations**
- Use Next.js API routes to build secure endpoints for CRUD operations:
  - Courses: Create, Read, Update, Delete
  - Sections: Add, Reorder, Mark Completed
  - Users: Fetch Profile, Update Progress

### **7. Search & Filter Courses**
- Add dynamic search functionality based on course title and category using Prisma queries.
- Build UI with TailwindCSS + Shadcn's components for filtering options.

### **8. Purchase Courses Using Stripe**
- Integrate Stripe for secure payment processing.
- Create a checkout page and webhooks to handle payment success/failure.
- Store purchase details in the database.

### **9. Authentication with Clerk**
- Implement sign-up and sign-in functionality using **Clerk**.
- Secure API routes with Clerk's middleware for authentication and user session management.

### **10. Rich Text Editor**
- Use a library like `@tiptap/react` or `react-quill` for rich-text editing.
- Enable instructors to format descriptions for courses and curriculum.

### **11. Instructor Performance Dashboard**
- Use a charting library like `react-chartjs-2` to create visualizations for instructor performance metrics (e.g., sales, enrollments).
- Fetch data dynamically and display KPIs.

### **12. Mark Sections Completed/Uncompleted**
- Allow users to mark individual sections as completed/uncompleted.
- Save progress in the database and dynamically update the UI.

### **13. Course Progress Calculation**
- Calculate progress percentage based on completed sections.
- Show progress bar on the course page.

### **14. Video Processing with Mux**
- Use Mux for video transcoding and streaming.
- Display videos using Mux's player for optimized playback.

---

## **Additional Steps**

### **1. Deployment**
- Deploy the app using **Vercel** (for frontend) and **Aiven** for MySQL.
- Set up environment variables for sensitive data (Stripe keys, Clerk API keys, etc.).

### **2. Testing**
- Write unit tests for key components and integration tests for APIs using Jest or Playwright.

### **3. Scalability**
- Optimize database queries and use Prisma's connection pooling.
- Implement caching strategies (e.g., Redis) for frequently accessed data.

---

This project combines modern web development practices to create a highly functional, feature-rich platform suitable for learners and instructors alike. Feel free to reach out for contributions or feedback!

