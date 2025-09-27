from reportlab.platypus import SimpleDocTemplate, Paragraph, Spacer
from reportlab.lib.styles import getSampleStyleSheet
from reportlab.lib.pagesizes import A4

file_name = "CRM_Jewel_Management_Developer_Document.pdf"
doc = SimpleDocTemplate(file_name, pagesize=A4)
styles = getSampleStyleSheet()
story = []

story.append(Paragraph("CRM Application for Jewel Management (Developer Document)", styles['Title']))
story.append(Spacer(1, 12))

sections = [
    ("1. Introduction", "This document outlines the development requirements, features, modules, and technical specifications for a CRM (Customer Relationship Management) application tailored for jewel management businesses. The CRM system aims to help jewelry retailers manage inventory, customers, orders, sales, suppliers, and communication efficiently."),
    ("2. Objectives", "- To centralize and automate jewelry store operations<br/>- To manage customer data, sales records, and inventory<br/>- To enable seamless communication between staff and customers<br/>- To support decision-making through reporting and analytics"),
    ("3. Key Features", "- Customer Management: Add, edit, delete customer profiles, track purchase history, preferences, and birthdays.<br/>- Inventory Management: Manage stock, categorize jewelry by type (gold, diamond, silver), track product movements, and set alerts for low stock.<br/>- Sales and Billing: Create invoices, manage discounts, GST calculations, and issue receipts.<br/>- Order Tracking: Status updates for custom and repair orders with estimated delivery dates.<br/>- Supplier Management: Manage supplier details, order history, and payment dues.<br/>- Notifications: Send SMS/Email reminders for orders, payments, birthdays, and promotions.<br/>- Reports & Analytics: Daily sales reports, inventory reports, customer insights.<br/>- User Roles and Access Control: Admin, Manager, Sales Staff roles with specific permissions."),
    ("4. Technical Stack", "- Frontend: React.js /Angular<br/>- Backend: Node.js / Django / Laravel<br/>- Database: MySQL / MongoDB<br/>- Authentication: JWT / OAuth 2.0<br/>- Hosting: AWS / Firebase / DigitalOcean<br/>- SMS/Email API: Twilio / SendGrid"),
    ("5. Modules", "1. Dashboard - Overview of sales, inventory, and customer activity<br/>2. Customers - Add/view/edit customers, Purchase history and follow-ups<br/>3. Inventory - Add/view/edit/delete items, Categories, tags, and barcodes<br/>4. Sales - New sale entries, Apply discounts/taxes, Generate invoice/receipt<br/>5. Orders - Track order status, Notify customers on update<br/>6. Suppliers - Manage purchase orders, Supplier profiles<br/>7. Reports - Filter by date, item, customer, Export in Excel/PDF format<br/>8. Settings - User roles and permissions, GST, invoice templates, etc."),
    ("6. Developer Guidelines", "- Follow MVC architecture<br/>- Ensure responsive UI for desktop and mobile<br/>- Use version control (Git)<br/>- Implement proper validation and error handling<br/>- Secure sensitive data (e.g., using HTTPS, encryption)"),
    ("7. Deployment & Maintenance", "- Initial deployment via CI/CD pipeline<br/>- Regular updates for bug fixes and new features<br/>- Automated backups and monitoring"),
    ("8. Future Enhancements", "- Mobile app integration<br/>- Loyalty points and rewards module<br/>- AI-based recommendation system<br/>- Multi-store support"),
    ("9. Conclusion", "This CRM application is designed to streamline jewelry business processes, enhance customer experience, and provide insightful data for growth. Developers are expected to maintain code quality, ensure usability, and support scalability.")
]

for title, body in sections:
    story.append(Paragraph(f"<b>{title}</b>", styles['Heading3']))
    story.append(Spacer(1, 6))
    story.append(Paragraph(body, styles['BodyText']))
    story.append(Spacer(1, 12))

doc.build(story)
print(f"PDF '{file_name}' created successfully.")
 Hulk
