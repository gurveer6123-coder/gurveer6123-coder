export default function GitHubPortfolioBanner() {
  return (
    <div className="min-h-screen bg-black text-white p-6 font-sans">
      <div className="max-w-7xl mx-auto border border-blue-900 rounded-3xl overflow-hidden shadow-2xl bg-gradient-to-br from-[#050816] to-[#02030a]">
        {/* Header */}
        <div className="grid grid-cols-1 lg:grid-cols-2 gap-8 p-10 border-b border-blue-900">
          <div className="flex flex-col md:flex-row items-center gap-8">
            <div className="relative">
              <img
                src="https://via.placeholder.com/260x260.png?text=Your+Photo"
                alt="profile"
                className="w-64 h-64 rounded-full border-4 border-blue-500 object-cover"
              />
              <div className="absolute bottom-5 right-4 w-6 h-6 rounded-full bg-green-500 border-2 border-black"></div>
            </div>

            <div>
              <h1 className="text-5xl font-bold mb-3">Gurveer Singh</h1>
              <h2 className="text-2xl text-blue-400 font-semibold mb-5">
                Networking & Systems Student
              </h2>

              <p className="text-gray-300 leading-8 max-w-xl text-lg">
                Aspiring Network & Systems Administrator passionate about
                designing, implementing and securing reliable IT
                infrastructures. Hands-on with Cisco networking, Windows
                Server and Azure. Building real-world lab projects and
                continuously learning.
              </p>

              <div className="flex flex-wrap gap-6 mt-6 text-gray-400">
                <div>📍 British Columbia, Canada</div>
                <div>📧 yourmail@gmail.com</div>
              </div>
            </div>
          </div>

          {/* Right Side */}
          <div className="hidden lg:flex items-center justify-center relative">
            <div className="absolute inset-0 bg-blue-500/10 blur-3xl rounded-full"></div>

            <div className="relative w-full h-full flex items-center justify-center">
              <div className="bg-[#0d1328] border border-blue-900 rounded-3xl p-8 w-full max-w-lg shadow-xl">
                <div className="space-y-4">
                  <div className="h-4 bg-blue-500/40 rounded w-3/4"></div>
                  <div className="h-4 bg-blue-500/20 rounded"></div>
                  <div className="h-4 bg-blue-500/20 rounded w-5/6"></div>
                </div>

                <div className="mt-10 grid grid-cols-4 gap-4">
                  {Array.from({ length: 8 }).map((_, i) => (
                    <div
                      key={i}
                      className="h-16 rounded-xl border border-blue-900 bg-[#0b1020] flex items-center justify-center text-blue-400"
                    >
                      ⚡
                    </div>
                  ))}
                </div>

                <div className="mt-8 border border-blue-900 rounded-2xl p-5 bg-black/30">
                  <p className="text-blue-300 font-mono text-lg leading-8">
                    {"> Connecting the world,"}
                    <br />
                    {"> one network at a time."}
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>

        {/* Main Content */}
        <div className="grid grid-cols-1 lg:grid-cols-2 gap-10 p-10">
          {/* About */}
          <div className="space-y-8">
            <div>
              <h2 className="text-3xl font-bold text-blue-400 mb-6">
                About Me
              </h2>

              <div className="space-y-5 text-gray-300 text-lg">
                <div className="flex gap-4">
                  <span>🎓</span>
                  <p>
                    Computer Science student focused on Networking & Systems
                  </p>
                </div>

                <div className="flex gap-4">
                  <span>🖧</span>
                  <p>
                    Hands-on with Cisco Networking, Windows Server & Azure
                  </p>
                </div>

                <div className="flex gap-4">
                  <span>💻</span>
                  <p>Building and documenting networking lab projects</p>
                </div>

                <div className="flex gap-4">
                  <span>🚀</span>
                  <p>Open to internships and new opportunities</p>
                </div>
              </div>
            </div>

            {/* Featured Repositories */}
            <div>
              <h2 className="text-3xl font-bold text-blue-400 mb-6">
                Featured Repositories
              </h2>

              <div className="space-y-5">
                {[
                  {
                    title: 'Network-Labs',
                    desc: 'Cisco networking configurations and topologies.',
                    tech: 'Cisco',
                  },
                  {
                    title: 'Windows-Server-Labs',
                    desc: 'Active Directory, DHCP, DNS and Group Policy labs.',
                    tech: 'PowerShell',
                  },
                  {
                    title: 'Azure-Labs',
                    desc: 'Azure cloud deployments and virtual networks.',
                    tech: 'Azure',
                  },
                ].map((repo, i) => (
                  <div
                    key={i}
                    className="border border-blue-900 rounded-2xl p-6 bg-[#070b16] hover:border-blue-500 transition"
                  >
                    <h3 className="text-2xl font-semibold text-blue-300 mb-2">
                      {repo.title}
                    </h3>

                    <p className="text-gray-400 mb-4">{repo.desc}</p>

                    <div className="flex items-center justify-between">
                      <span className="text-blue-400">● {repo.tech}</span>
                      <span className="text-gray-500">★</span>
                    </div>
                  </div>
                ))}
              </div>
            </div>
          </div>

          {/* Right Column */}
          <div className="space-y-10">
            {/* Tech Stack */}
            <div>
              <h2 className="text-3xl font-bold text-blue-400 mb-6">
                Tech Stack
              </h2>

              <div className="grid grid-cols-2 md:grid-cols-3 gap-5">
                {[
                  'Cisco',
                  'Windows Server',
                  'Azure',
                  'Linux',
                  'Security+',
                  'TCP/IP',
                  'VLAN',
                  'DHCP',
                  'DNS',
                ].map((item) => (
                  <div
                    key={item}
                    className="border border-blue-900 bg-[#070b16] rounded-2xl p-5 text-center hover:border-blue-500 transition"
                  >
                    <div className="text-3xl mb-3">⚙️</div>
                    <div className="text-gray-300">{item}</div>
                  </div>
                ))}
              </div>
            </div>

            {/* Stats */}
            <div>
              <h2 className="text-3xl font-bold text-blue-400 mb-6">
                GitHub Stats
              </h2>

              <div className="grid grid-cols-2 gap-5">
                {[
                  ['25+', 'Repositories'],
                  ['18+', 'Projects'],
                  ['70+', 'Commits'],
                  ['15+', 'Contributions'],
                ].map(([num, label]) => (
                  <div
                    key={label}
                    className="border border-blue-900 bg-[#070b16] rounded-2xl p-6"
                  >
                    <div className="text-4xl font-bold text-blue-400 mb-2">
                      {num}
                    </div>
                    <div className="text-gray-400">{label}</div>
                  </div>
                ))}
              </div>
            </div>

            {/* Learning */}
            <div>
              <h2 className="text-3xl font-bold text-blue-400 mb-6">
                Currently Learning
              </h2>

              <ul className="space-y-4 text-lg text-gray-300">
                <li>• Advanced Routing & Switching</li>
                <li>• Azure Administration</li>
                <li>• Cybersecurity (Security+)</li>
                <li>• Python for Automation</li>
              </ul>
            </div>

            {/* Connect */}
            <div>
              <h2 className="text-3xl font-bold text-blue-400 mb-6">
                Connect With Me
              </h2>

              <div className="space-y-4 text-lg text-gray-300">
                <div>🌐 github.com/yourusername</div>
                <div>💼 linkedin.com/in/yourprofile</div>
                <div>📧 yourmail@gmail.com</div>
              </div>
            </div>
          </div>
        </div>

        {/* Footer */}
        <div className="border-t border-blue-900 p-8 text-center">
          <p className="text-2xl text-blue-300 italic">
            “The best way to predict the future is to build it.”
          </p>
          <p className="text-gray-500 mt-3">— Peter Drucker</p>
        </div>
      </div>
    </div>
  )
}
