# SalesGear-Realty-and-Advisory-
{
  "name": "salesgear-realty",
  "version": "1.0.0",
  "private": true,
  "scripts": {
    "dev": "next dev",
    "build": "next build",
    "start": "next start",
    "lint": "next lint"
  },
  "dependencies": {
    "next": "15.3.3",
    "react": "^19.0.0",
    "react-dom": "^19.0.0",
    "framer-motion": "^12.16.0",
    "lucide-react": "^0.525.0"
  },
  "devDependencies": {
    "@types/node": "^22.15.30",
    "@types/react": "^19.1.8",
    "@types/react-dom": "^19.1.6",
    "autoprefixer": "^10.4.21",
    "eslint": "^9.29.0",
    "eslint-config-next": "15.3.3",
    "postcss": "^8.5.6",
    "tailwindcss": "^3.4.17",
    "typescript": "^5.8.3"
  }
}import "./globals.css";
import type { Metadata } from "next";

export const metadata: Metadata = {
  title: "SalesGear Realty & Advisory",
  description:
    "Pune's Trusted Sole Selling & Mandate Partner. From Inventory to Sold Out.",
};

export default function RootLayout({
  children,
}: {
  children: React.ReactNode;
}) {
  return (
    <html lang="en">
      <body>{children}</body>
    </html>
  );
}
/* Reset */

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Smooth Scroll */

html {
  scroll-behavior: smooth;
}

/* Body */

body {
  font-family: Arial, Helvetica, sans-serif;
  background: #f8fbff;
  color: #222;
  overflow-x: hidden;
}

/* Headings */

h1,
h2,
h3,
h4 {
  font-weight: 700;
}

p {
  line-height: 1.7;
}

/* Links */

a {
  text-decoration: none;
  color: inherit;
}

/* Buttons */

button {
  transition: 0.3s ease;
}

button:hover {
  transform: translateY(-3px);
  opacity: 0.95;
}

/* Section */

section {
  width: 100%;
}

/* Container */

.container {
  width: 90%;
  max-width: 1200px;
  margin: auto;
}

/* Cards */

.card {
  background: white;
  border-radius: 18px;
  box-shadow: 0 12px 30px rgba(0,0,0,0.08);
  padding: 30px;
  transition: 0.3s;
}

.card:hover {
  transform: translateY(-8px);
}

/* Blue Button */

.btn-primary {
  background: #0F4CDB;
  color: white;
  padding: 14px 28px;
  border-radius: 10px;
  border: none;
  cursor: pointer;
}

/* Orange Button */

.btn-secondary {
  background: #F97316;
  color: white;
  padding: 14px 28px;
  border-radius: 10px;
  border: none;
  cursor: pointer;
}

/* Footer */

footer {
  margin-top: 50px;
}

/* Responsive */

@media (max-width:768px){

h1{
font-size:36px !important;
}

h2{
font-size:28px !important;
}

p{
font-size:16px !important;
}

}
"use client";

import Link from "next/link";

export default function Navbar() {
  return (
    <header
      style={{
        position: "sticky",
        top: 0,
        zIndex: 1000,
        background: "rgba(255,255,255,0.95)",
        backdropFilter: "blur(10px)",
        boxShadow: "0 2px 12px rgba(0,0,0,0.08)",
      }}
    >
      <nav
        style={{
          maxWidth: "1200px",
          margin: "0 auto",
          display: "flex",
          justifyContent: "space-between",
          alignItems: "center",
          padding: "18px 20px",
        }}
      >
        <div>
          <h2
            style={{
              color: "#0F4CDB",
              margin: 0,
              fontSize: "28px",
              fontWeight: 700,
            }}
          >
            SalesGear Realty
          </h2>
        </div>

        <div
          style={{
            display: "flex",
            gap: "25px",
            alignItems: "center",
            fontWeight: 600,
          }}
        >
          <Link href="/">Home</Link>
          <Link href="/about">About</Link>
          <Link href="/services">Services</Link>
          <Link href="/projects">Projects</Link>
          <Link href="/contact">Contact</Link>

          <a
            href="https://wa.me/917558299969"
            target="_blank"
            style={{
              background: "#25D366",
              color: "#fff",
              padding: "10px 18px",
              borderRadius: "8px",
              textDecoration: "none",
              fontWeight: "bold",
            }}
          >
            WhatsApp
          </a>
        </div>
      </nav>
    </header>
  );
}
export default function Services() {
  const services = [
    {
      title: "Exclusive Sales Mandate",
      description:
        "Complete sales management for residential and commercial projects.",
      icon: "🏢",
    },
    {
      title: "Project Launch Strategy",
      description:
        "Launch planning, pricing strategy and market positioning.",
      icon: "🚀",
    },
    {
      title: "Digital Marketing",
      description:
        "Meta Ads, Google Ads, social media campaigns and lead generation.",
      icon: "📱",
    },
    {
      title: "Channel Partner Network",
      description:
        "Strong CP network across Pune for faster inventory movement.",
      icon: "🤝",
    },
    {
      title: "Dedicated Sales Team",
      description:
        "Professional site sales team with CRM and reporting.",
      icon: "👥",
    },
    {
      title: "CRM & Sales Reporting",
      description:
        "Daily MIS, enquiry tracking and booking reports.",
      icon: "📊",
    },
  ];

  return (
    <section
      style={{
        padding: "80px 20px",
        background: "#f8fbff",
      }}
    >
      <div
        style={{
          maxWidth: "1200px",
          margin: "auto",
        }}
      >
        <h2
          style={{
            textAlign: "center",
            color: "#0F4CDB",
            fontSize: "42px",
            marginBottom: "15px",
          }}
        >
          Our Services
        </h2>

        <p
          style={{
            textAlign: "center",
            color: "#666",
            marginBottom: "50px",
            fontSize: "18px",
          }}
        >
          End-to-End Sales & Marketing Solutions for Real Estate 
          <Services />
          export default function Stats() {
  const stats = [
    {
      value: "₹500+ Cr",
      label: "Inventory Managed",
    },
    {
      value: "1000+",
      label: "Units Marketed",
    },
    {
      value: "25+",
      label: "Developer Partners",
    },
    {
      value: "5000+",
      label: "Customer Enquiries",
    },
  ];

  return (
    <section
      style={{
        background: "#0F4CDB",
        color: "#fff",
        padding: "80px 20px",
      }}
    >
      <div
        style={{
          maxWidth: "1200px",
          margin: "auto",
        }}
      >
        <h2
          style={{
            textAlign: "center",
            fontSize: "42px",
            marginBottom: "15px",
          }}
        >
          Our Achievements
        </h2>

        <p
          style={{
            textAlign: "center",
            marginBottom: "50px",
            opacity: 0.9,
          }}
        >
          Delivering results that developers trust.
        </p>

        <div
          style={{
            display: "grid",
            gridTemplateColumns: "repeat(auto-fit,minmax(220px,1fr))",
            gap: "25px",
          }}
        >
          {stats.map((item, index) => (
            <div
              key={index}
              style={{
                background: "rgba(255,255,255,0.1)",
                borderRadius: "15px",
                padding: "35px",
                textAlign: "center",
                backdropFilter: "blur(10px)",
              }}
            >
              <h3
                style={{
                  fontSize: "42px",
                  marginBottom: "10px",
                  color: "#fff",
                }}
              >
                {item.value}
              </h3>

              <p
                style={{
                  fontSize: "18px",
                  opacity: 0.95,
                }}
              >
                {item.label}
              </p>
            </div>
          ))}
        </div>
      </div>
    </section>
  );
} ji
export default function Projects() {
  const projects = [
    {
      name: "T5E - The 5 Elements",
      location: "Wagholi, Pune",
      type: "1, 2 & 3 BHK",
      price: "Starting ₹41 Lakhs",
      image:
        "https://images.unsplash.com/photo-1600585154340-be6161a56a0c?w=1200&q=80",
    },
    {
      name: "Siddhivinayak Vishwa",
      location: "Wagholi, Pune",
      type: "2 & 3 BHK",
      price: "Premium Homes",
      image:
        "https://images.unsplash.com/photo-1460317442991-0ec209397118?w=1200&q=80",
    },
    {
      name: "Upcoming Premium Project",
      location: "Pune",
      type: "Luxury Apartments",
      price: "Coming Soon",
      image:
        "https://images.unsplash.com/photo-1512917774080-9991f1c4c750?w=1200&q=80",
    },
  ];

  return (
    <section
      style={{
        padding: "90px 20px",
        background: "#ffffff",
      }}
    >
      <div
        style={{
          maxWidth: "1200px",
          margin: "0 auto",
        }}
      >
        <h2
          style={{
            textAlign: "center",
            color: "#0F4CDB",
            fontSize: "42px",
            marginBottom: "15px",
          }}
        >
          Featured Projects
        </h2>

        <p
          style={{
            textAlign: "center",
            color: "#666",
            marginBottom: "50px",
          }}
        >
          Explore some of our exclusive real estate projects.
        </p>

        <div
          style={{
            display: "grid",
            gridTemplateColumns: "repeat(auto-fit,minmax(320px,1fr))",
            gap: "30px",
          }}
        >
          {projects.map((project, index) => (
            <div
              key={index}
              style={{
                background: "#fff",
                borderRadius: "18px",
                overflow: "hidden",
                boxShadow: "0 12px 30px rgba(0,0,0,0.1)",
              }}
            >
              <img
                src={project.image}
                alt={project.name}
                style={{
                  width: "100%",
                  height: "220px",
                  objectFit: "cover",
                }}
              />

              <div style={{ padding: "25px" }}>
                <h3
                  style={{
                    color: "#0F4CDB",
                    marginBottom: "10px",
                  }}
                >
                  {project.name}
                </h3>

                <p>📍 {project.location}</p>
                <p>🏠 {project.type}</p>
                <p
                  style={{
                    fontWeight: "bold",
                    color: "#F97316",
                    margin: "15px 0",
                  }}
                >
                  {project.price}
                </p>

                <button
                  style={{
                    background: "#0F4CDB",
                    color: "#fff",
                    border: "none",
                    padding: "12px 24px",
                    borderRadius: "8px",
                    cursor: "pointer",
                    width: "100%",
                  }}
                >
                  View Details
                </button>
              </div>
            </div>
          ))}
        </div>
      </div>
    </section>
  );
}export default function Contact() {
  return (
    <section
      style={{
        padding: "80px 20px",
        background: "#F8FBFF",
      }}
    >
      <div
        style={{
          maxWidth: "1200px",
          margin: "0 auto",
          display: "grid",
          gridTemplateColumns: "repeat(auto-fit,minmax(350px,1fr))",
          gap: "50px",
          alignItems: "center",
        }}
      >
        <div>
          <h2
            style={{
              color: "#0F4CDB",
              fontSize: "42px",
              marginBottom: "20px",
            }}
          >
            Contact SalesGear Realty
          </h2>

          <p
            style={{
              color: "#666",
              marginBottom: "30px",
              lineHeight: "1.8",
            }}
          >
            Ready to launch your project or looking for a trusted Sole Selling
            Partner? Contact us today.
          </p>

          <p style={{ marginBottom: "15px" }}>
            📞 <strong>+91 75582 99969</strong>
          </p>

          <p style={{ marginBottom: "15px" }}>
            ✉️ salesgearrealty@gmail.com
          </p>

          <p style={{ marginBottom: "25px" }}>
            📍 Wagholi, Pune
          </p>

          <a
            href="https://wa.me/917558299969"
            target="_blank"
            style={{
              background: "#25D366",
              color: "#fff",
              padding: "14px 28px",
              borderRadius: "10px",
              textDecoration: "none",
              fontWeight: "bold",
            }}
          >
            Chat on WhatsApp
          </a>
        </div>

        <div
          style={{
            background: "#fff",
            padding: "35px",
            borderRadius: "16px",
            boxShadow: "0 10px 25px rgba(0,0,0,.08)",
          }}
        >
          <h3
            style={{
              marginBottom: "25px",
              color: "#0F4CDB",
            }}
          >
            Send an Enquiry
          </h3>

          <input
            placeholder="Full Name"
            style={inputStyle}
          />

          <input
            placeholder="Mobile Number"
            style={inputStyle}
          />

          <input
            placeholder="Email Address"
            style={inputStyle}
          />

          <textarea
            placeholder="Message"
            rows={5}
            style={inputStyle}
          />

          <button
            style={{
              width: "100%",
              background: "#0F4CDB",
              color: "#fff",
              padding: "15px",
              border: "none",
              borderRadius: "10px",
              cursor: "pointer",
              fontWeight: "bold",
              fontSize: "16px",
            }}
          >
            Submit Enquiry
          </button>
        </div>
      </div>
    </section>
  );
}

const inputStyle = {
  width: "100%",
  padding: "14px",
  marginBottom: "15px",
  borderRadius: "10px",
  border: "1px solid #ddd",
  fontSize: "16px",
} as const;
import Link from "next/link";

export default function Footer() {
  return (
    <footer
      style={{
        background: "#0B1F4D",
        color: "#fff",
        padding: "70px 20px 25px",
        marginTop: "60px",
      }}
    >
      <div
        style={{
          maxWidth: "1200px",
          margin: "0 auto",
          display: "grid",
          gridTemplateColumns: "2fr 1fr 1fr 1fr",
          gap: "40px",
        }}
      >
        <div>
          <h2
            style={{
              color: "#fff",
              marginBottom: "15px",
            }}
          >
            SalesGear Realty & Advisory
          </h2>

          <p
            style={{
              lineHeight: "1.8",
              color: "#d1d5db",
            }}
          >
            Pune's Trusted Sole Selling & Mandate Partner helping developers
            launch, market and sell projects through strategic marketing,
            dedicated sales teams and complete sales management.
          </p>
        </div>

        <div>
          <h3 style={{ marginBottom: "20px" }}>Quick Links</h3>

          <p><Link href="/">Home</Link></p>
          <p><Link href="/about">About</Link></p>
          <p><Link href="/services">Services</Link></p>
          <p><Link href="/projects">Projects</Link></p>
          <p><Link href="/contact">Contact</Link></p>
        </div>

        <div>
          <h3 style={{ marginBottom: "20px" }}>Services</h3>

          <p>Exclusive Sales Mandate</p>
          <p>Project Launch</p>
          <p>Digital Marketing</p>
          <p>CRM Management</p>
          <p>Channel Partner Network</p>
        </div>

        <div>
          <h3 style={{ marginBottom: "20px" }}>Contact</h3>

          <p>📞 +91 75582 99969</p>
          <p>✉️ salesgearrealty@gmail.com</p>
          <p>📍 Wagholi, Pune</p>
        </div>
      </div>

      <hr
      
