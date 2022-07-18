# Ed-Fi Analytics Middle Tier

This project contains migration scripts that will install the ODS Analytics
Middle Tier into an Ed FI ODS v2.x database.

* [Overview](#overview)
* [Installing and Configuring the Analytics Middle Tier](#installing-and-configuring-the-analytics-middle-tier)
* [Building Solutions Using the Analytics Middle Tier](#building-solutions-using-the-analytics-middle-tier)
* [Contributing to the Codebase](#contributing-to-the-codebase)
* [Roadmap](#roadmap)
* [Support](#support)
* [License](#license)

## Overview

The project includes views, tables, and indexes to satisfy (a) an Early Warning
System use case, and (b) provide a few extra dimension tables that may be useful
for analytics data modelers. The views are the core of this project.

See [Analytics Middle Tier Design](docs/design.md) for more information on the
background for this project, requirements, and design principles.

## Installing and Configuring the Analytics Middle Tier

1. Download the [latest
   release](https://github.com/Ed-Fi-Alliance/Ed-Fi-X-Analytics-Middle-Tier/releases)
   of the compiled executable (`EdFi.AnalyticsMiddleTier-win10.x64.zip`).
2. Unzip the archive.
3. Open a command prompt and CD to the directory containing the unzipped
   contents.
4. Run the following command, substituting in a correct connection string for
   your database:

   ```powershell
   .\EdFi.AnalyticsMiddleTier.Console.exe --connectionString "Server=.;Database=EdFi_Glendale;Trusted_connection=true"
   ```

5. Start writing queries against the views in the `analytics` schema.

See [Installing the Ed-Fi Analytics Middle Tier](docs/installation.md) for
more command-line options, uninstall, and next steps.

## Building Solutions Using the Analytics Middle Tier

For additional information on building solutions from these views, see

* [Dimensional Views](docs/dimensional-views.md): descriptions of each
  dimensional view available in the Analytics Middle Tier.
* [Patterns and Practices](docs/patterns-and-practices.md): guidance and
  considerations related to performance and security.
* [Early Warning System](docs/early-warning-system.md): descriptions of the
  early warning system data model, and additional related scripts provided in
  the [samples](samples/) directory.

## Contributing to the Codebase

While code contributions are invited, no formal mechanism is in place beyond
submitting a pull request. Please review the [Solution
Architecture](docs/solution.md) for information on the source code organization,
naming conventions, testing, and continuous integration.

## Roadmap

The only solid plan is an MVP release supporting the 2.x data model in time for
the Ed-Fi Summit in October 2018. Beyond this, the Alliance will consider
additions such as (no commitment!):

* Assessments
* Dimension or fact views requested by the community
* 3.x data model

## Support

These scripts are provided as-is, but the Alliance welcomes feedback on
additions or changes that would make these resources more user friendly.
Feedback is best shared by raising a ticket on the Ed-Fi Tracker [Exchange
Contributions Project](https://tracker.ed-fi.org/projects/EXC/). We invite [pull
requests](https://github.com/Ed-Fi-Alliance/Analytics-Middle-Tier) with
corrections and proposed additions! :yellow_heart:

## License

Copyright (c) 2019 Ed-Fi Alliance, LLC and contributors.

Licensed under the [Apache License, Version 2.0](LICENSE) (the "License").

Unless required by applicable law or agreed to in writing, software distributed
under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
CONDITIONS OF ANY KIND, either express or implied. See the License for the
specific language governing permissions and limitations under the License.

See [NOTICES](NOTICES.md) for additional copyright and license notifications.