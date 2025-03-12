# pantheon-consolidate
export default function HomePage() {
 const services = [
   "Bathroom Renovations", "Leak Detection", "Drain Cleaning", "Toilet Repairs", "Shower Installations",
   "Pipe Relining", "Geyser Installations", "Water Pressure Fixes", "Septic Tank Services", "Plumbing Inspections",
   "Emergency Plumbing", "Solar Water Heating", "Backflow Prevention", "Water Filtration Systems",
   "Kitchen Plumbing", "Outdoor Plumbing", "Greywater Recycling", "Underfloor Heating Installation",
   "Rainwater Harvesting", "Jacuzzi & Spa Installations"
 ];

 return (
   <div className="min-h-screen bg-gray-50 text-gray-900">
     {/* Header Section */}
     <header className="w-full bg-gray-900 text-white py-6 flex justify-between items-center px-8 shadow-lg">
       <h1 className="text-3xl font-bold">Pantheon Consolidated</h1>
       <a
         href="https://wa.me/2762793755"
         target="_blank"
         rel="noopener noreferrer"
         className="bg-green-500 px-5 py-3 rounded-lg shadow-md hover:bg-green-600"

         WhatsApp Us
       </a>
     </header>

     <div className="flex flex-col items-center justify-center p-10">
       <h1 className="text-5xl font-bold text-gray-800">Welcome to Pantheon Consolidated</h1>
       <p className="mt-4 text-lg text-gray-700 text-center">Plumbing & Bathroom Renovation Experts in Pretoria, South Africa</p>
       <p className="mt-2 text-md text-gray-600">Visit us at <a href="https://pantheonconsolidated.co.za" className="text-blue-500 underline">pantheonconsolidated.co.za</a></p>
       <p className="mt-1 text-md text-gray-600">Contact: <span className="font-bold">076 279 3755</span></p>
       <p className="mt-1 text-md text-gray-600">Email: <a href="mailto:pantheonconsolidated@gmail.com" className="text-blue-500 underline">pantheonconsolidated@gmail.com</a></p>

       <div className="mt-8 w-full max-w-4xl grid grid-cols-2 gap-6">
         <img src="/images/blocked-drain.jpg" alt="Blocked Drain" className="rounded-lg shadow-md" />
         <img src="/images/fancy-bathroom.jpg" alt="Fancy Bathroom" className="rounded-lg shadow-md" />
       </div>

       <h2 className="mt-10 text-3xl font-semibold text-gray-800">Our Services</h2>
       <ul className="mt-6 grid grid-cols-2 md:grid-cols-3 gap-6 text-gray-700 text-lg">
         {services.map((service, index) => (
           <li key={index} className="bg-white p-4 shadow-md rounded-lg border border-gray-200">{service}</li>
         ))}
       </ul>

       <h2 className="mt-10 text-3xl font-semibold text-gray-800">Schedule an Appointment</h2>
       <button className="mt-6 px-8 py-4 bg-gray-900 text-white rounded-lg shadow-md hover:bg-gray-700">
         Book Now
       </button>
     </div>
   </div>
 );
}
