# MANDATE — Global Power Simulator v0.8

A self-contained, mobile-friendly browser strategy game where one player can control governments, legal opposition parties, illegal political organizations, and multinational companies inside the same shared world.

No framework, build step, API key, or database is required.

## Run locally

Open `index.html` in a modern browser.

For more reliable browser storage, run a local server from the folder containing the game:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Deploy on GitHub Pages

1. Create a public GitHub repository.
2. Upload `index.html` to the repository root.
3. Open **Settings → Pages**.
4. Select **Deploy from a branch**.
5. Choose `main` and `/root`, then save.



## Government management in v0.8

National leaders now have a dedicated **Government** tab with five organized sections: Cabinet, Ministry Budgets, Public Workforce, Security & Intelligence, and Political Crises.

### Cabinet and government composition

- Eleven ministries with individually appointed ministers
- Minister competence, loyalty, integrity, ambition, ideology, and professional background
- Appoint candidates, replace incumbents, dismiss ministers, or leave a ministry vacant
- Cabinet composition summaries for technocrats, political loyalists, security figures, and reformers
- Vacancies and weak ministers reduce delivery, coordination, revenue collection, and institutional performance
- Ministers can lose loyalty, become implicated in corruption, threaten resignation, or become liabilities during crises

### Ministry budgets and priorities

- Increase or reduce the complete recurring government-program envelope as a share of GDP
- Redistribute a fixed 100% allocation among ministries and a contingency reserve
- Separate annual budgets for finance, health, education, interior, defense, intelligence, housing and social protection, science and culture, infrastructure, environment, and state administration
- Six executive priorities: balanced government, growth, human development, security, welfare, and climate resilience
- Budget levels combine with staffing, salaries, minister competence, integrity, corruption, and executive priority to determine ministry performance

### Public-sector workforce

The player can raise or reduce staffing and salaries for:

- Teachers
- Doctors and nurses
- Police and emergency personnel
- Armed-forces personnel
- Civil servants
- Intelligence officers
- Researchers and scientists
- Social and housing workers

Changes create permanent monthly payroll costs or savings. Staffing and pay affect morale, strikes, unemployment, inflation, service quality, approval, and stability.

### Security and intelligence

- Manage security around the head of state or government
- Increase or reduce intelligence funding
- Increase or reduce counterintelligence capacity
- Track leadership threats, hostile-service penetration, insider leaks, and recurring fiscal costs
- Excessive security spending can reduce democratic integrity, while weak funding increases hidden exposure

### Political crises

The government can face:

- Procurement and corruption scandals
- Ministerial resignation threats
- Public-sector strikes
- Intelligence and counterintelligence failures
- Coalition revolts and legislative crises

Unresolved crises worsen approval, political capital, stability, and election prospects every month. Each crisis provides several responses with different fiscal, political, institutional, and corruption consequences.

## National data engine in v0.7

Every one of the eight playable countries now carries a structured model with **1,336 tracked numeric variables**. The new **Nation Data** tab is available to governments, opposition parties, underground organizations, and companies for the country where the active entity is based.

### Data domains

- GDP, GDP per capita, real and nominal growth, inflation, unemployment, productivity, wages, poverty, inequality, HDI, investment, savings, and 12 economic sectors
- Population growth, fertility, mortality, life expectancy, migration, urbanization, 18 five-year age cohorts, sex distribution, labor participation, and 12 modeled regions
- Revenue sources, spending programs, debt, deficit, debt service, credit quality, government assets, liabilities, tax compliance, evasion, and execution quality
- Exports, imports, trade balance, FDI, reserves, customs, export complexity, and 12 foreign-partner groups
- Ten energy sources with generation, capacity, cost, reliability, emissions, reserves, investment, and import dependence
- Policy rates, bank rates, sovereign yields, currencies, stock markets, housing, bank assets, bad loans, capital, pensions, and financial inclusion
- Crime, organized crime, terrorism, cyber threats, borders, police, prisons, intelligence, unrest, separatism, food, water, disasters, and pandemic readiness
- Health, education, welfare, literacy, enrollment, research, academic freedom, medical access, health outcomes, and rural gaps
- Six military branches with personnel, readiness, modernization, logistics, training, morale, maintenance, command, deployability, cyber integration, and reserves
- Eight political-party families, institutions, elections, law, media, civil liberties, corruption, religious influence, and regional tension
- Faith groups and 20 social-regulation areas covering enforcement, public support, restrictiveness, and controversy
- Pollution, emissions, forests, biodiversity, water, climate risks, renewable energy, green investment, adaptation, transport, buildings, and disaster losses
- Ten sports and ten scientific fields, plus culture, tourism, creative exports, technology, startups, patents, research, universities, and global influence

All country models continue evolving each month, including countries that are not currently selected.

### Reports and spoken briefings

The game now has a procedural national-report engine. It combines live variables, sections, trends, countries, dates, and outcomes to support more than **184,000 fact combinations** and **24,000 article variants**. Generated reports are archived in the save and can be read aloud with the browser's installed speech voices.

These figures describe procedural combinations, not 184,000 individually hand-entered facts or 24,000 separately authored articles. The static browser build also does not contain studio-recorded dialogue; speech is generated through the Web Speech API when the browser supports it.

## Global power update in v0.6

### Playable roles

The starting role can be:

- President
- Prime minister
- King
- Queen
- Leader of a legal opposition party
- Leader of an illegal revolutionary organization
- Leader of an illegal separatist organization
- Leader of an underground democratic or exiled resistance network
- CEO of a multinational company

### Multiple entities in one save

The **Entities** tab supports up to 12 simultaneously controlled actors.

You can:

- Add governments in other playable countries
- Add several political parties
- Add several underground organizations
- Own and manage several multinational companies
- Switch control immediately through the top entity selector
- Give every entity one major strategic action each month
- Release non-primary entities from the portfolio

Every controlled entity continues evolving when another entity is active.

### Full multi-country government switching

Every controlled government has a separate national state, including:

- GDP, growth, inflation, unemployment, debt, treasury, and taxation
- Central-bank rates and delayed monetary transmission
- Bills, enacted laws, resolutions, and repeal history
- Infrastructure, energy, industrial, and public-service projects
- Long-term national plans
- Approval, legislature, elites, stability, corruption, and opposition
- Election or succession timing
- Country-specific history and economic trends

Switching governments saves the current country and loads the selected country’s complete national workspace. Other controlled countries continue moving through the lighter shared-world simulation while not selected.

### Legal opposition gameplay

Opposition parties track:

- National polling
- Legislative seats
- Campaign funds
- Party organization
- Credibility
- Media reach
- Government pressure
- Election schedule and victories

Available operations include rallies, investigations, coalition negotiations, media campaigns, governing platforms, and election-monitor training. Winning an election transforms the party into a government rather than ending the game.

### Underground organization gameplay

Illegal organizations track:

- Popular support
- Active cells
- Funds
- Secrecy
- Political legitimacy
- State heat
- Repression
- Autonomy or settlement progress

Operations are represented as abstract political strategy choices involving recruitment, manifestos, civil resistance, external sponsorship, secret negotiations, and escalation. The simulation models legitimacy, repression, exposure, and civilian consequences without providing real operational instructions.

A sufficiently strong organization can reach a negotiated settlement or take power after state collapse, converting it into a government.

### Multinational company gameplay

Companies track:

- Annual revenue and profit
- Valuation
- Cash and corporate debt
- Employees
- Innovation
- Reputation
- Market share
- Political influence
- Countries of operation

Corporate operations include factories, long-term research, lobbying, acquisitions, new-market entry, and bond issuance. Companies can affect employment, corruption, regulation, and national business conditions.

### Political continuity

Losing an election or being removed from government no longer automatically ends the game. The former administration becomes a controlled legal opposition party. Other countries and companies in the portfolio continue operating.

## Existing national systems

### Projects and industrialization

The separate **Projects** tab includes:

- Public transport and metropolitan railways
- Intercity passenger and freight railways
- Highways, expressways, airports, ports, and rural roads
- Solar, wind, nuclear, gas, hydroelectric, geothermal, grid, and storage projects
- Industrial parks, semiconductors, steel, automotive, food processing, pharmaceuticals, shipbuilding, and technology hubs
- Hospitals, schools, housing, water systems, digital government, and climate defenses

Projects have multi-year schedules, monthly costs, overruns, delays, incidents, construction capacity, maintenance, cancellation losses, and permanent effects.

### Monetary and long-term planning

- Raise, cut, or hold the central-bank policy rate
- Deposit, mortgage, business-loan, consumer-credit, and sovereign rates
- Delayed effects lasting up to 30 months
- Inflation expectations, credit, housing, banking health, investment, jobs, and currency effects
- Eight national plans lasting 6–12 years with annual milestones

### Legislation

- 30 legislative proposals
- 25 permanent bills that can become laws
- 5 one-time resolutions
- Separate Bills and Laws tabs
- Search, filters, voting strategies, failed votes, enactment dates, and repeal votes

### Base simulation

- Eight playable countries
- Monthly GDP, GDP per capita, growth, inflation, unemployment, revenue, spending, debt, and interest costs
- Elections, succession contests, party congresses, scandals, political removal, and crises
- Country rankings and a shared-world timeline
- Automatic local browser saving
- Existing-save migration
- Responsive desktop and mobile interface

## Testing completed

- Embedded JavaScript syntax validation
- All four starting-role flows
- Entity creation, switching, and removal
- One action per entity per month
- Company, opposition, underground, and secondary-government simulations
- Full national-state switching between controlled governments
- Access control for government-only systems
- Election loss continuing as opposition
- 84-month simulation with four simultaneous entities
- 1,336-variable model verified for all eight countries
- All 11 Nation Data views rendered without undefined or NaN values
- 36-month national-data evolution and procedural-report test
- Cabinet appointment, replacement, dismissal, and vacancy flows
- Eleven ministry budgets, total spending-envelope controls, and priority changes
- Eight public-worker staffing and salary systems
- Head-of-state security, intelligence, and counterintelligence controls
- Crisis generation, escalation, and response choices
- v0.7 save migration into the v0.8 government model
- 24-month government-management simulations across all eight countries
- Desktop and mobile layouts
- No runtime errors, NaN values, or undefined economic values in the tested flows

## Current limitation

This remains a serverless single-player build. The shared world contains simulated actors controlled by one player. Real accounts, online multiplayer, cloud saves, public leaderboards, and cross-device worlds require a backend and database.

## Data note

Starting values and economic relationships are simplified game baselines inspired by real macroeconomic systems. They are simulation values, not exact live forecasts or financial advice.
