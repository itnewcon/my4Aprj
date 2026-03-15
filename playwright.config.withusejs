const { defineConfig } = require('@playwright/test');

module.exports = defineConfig({
  testDir: './tests',
  retries: 1,
  timeout: 30000,
  workers: 3, // Parallel execution
  reporter: [['html', { open: 'never' }]],

  use: {
    baseURL: 'http://localhost:3000',
    headless: true,
  },

  projects: [
    { name: 'Chromium', use: { browserName: 'chromium' } },
    { name: 'Firefox', use: { browserName: 'firefox' } },    
  ],
  
});