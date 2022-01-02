# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.14.0] - ???

### Added
- Method `GetSummaryReportAsync` to get summary report.

## [1.13.0] - 18.11.2021

### Added
- Method `DeleteClientAsync` to delete client.

## [1.12.0] - 08.11.2021

### Added
- Now API URL, Experimental API URL and Reports API URL can be set in constructor.

## [1.11.1] - 16.10.2021

### Fixed
-  Fix related to error `Error converting value "NOT_REGISTERED"` (PR#53)

## [1.11.0] - 21.07.2021

### Added
- Method `GetDetailedReportAsync` to get detailed report form report API

## [1.10.0] - 15.07.2021

### Added
- Support for tags in `FindAllTimeEntriesForUserAsync`
- Method `UpdateClientNameAsync` to update name of the client
- Method `AddWorkspaceUser` to add user to workspace

## [1.9.0] - 07.06.2021

### Added
- Method `UpdateProjectEstimatesAsync` to `ClockifyClient`
- Method `UpdateProjectMembershipsAsync` to `ClockifyClient`


## [1.8.1] - 21.03.2021

### Fixed
- Issue #38 - Now UserStatus enum is deserialized correctly

## [1.8.0] - 21.03.2021

### Added
- Method `UpdateProjectAsync` to `ClockifyClient`

## [1.7.0] - 18.01.2020

### Added
- Support for paging in `FindAllUsersOnWorkspaceAsync`
- Support for paging in `FindAllClientsOnWorkspaceAsync`

## [1.6.0] - 02.12.2020

### Added
- Method `CreateTimeEntryForAnotherUserAsync` to `ClockifyClient`


## [1.5.0] - 27.10.2020

### Added
- Method `FindProjectByIdAsync` to `ClockifyClient`
- Method `FindAllTimeEntriesForProjectAsync` to `ClockifyClient`


## [1.4.0] - 24.09.2020

### Added
- Property `ClientId` and `ClientName`  to the `TimeEntryDtoImpl` (PR #20)

## [1.3.0]

### Added
- Support for query parameter in `FindAllWorkspacesAsync()` (PR #17)

## [1.2.0]

### Added
 - Support for deleting and updating tasks. (PR #16)
 - `Note` field to ProjectRequest and ProjectDtoImpl (PR #15)
 - `FindAllHydratedTimeEntriesForUserAsync` method to client (PR #12)
### Changed
- JsonSerializer to Json.Net
### Fixed
- `EstimateRequest` should now work properly. 

## [1.1.4]

### Fixed
- `Estimate` deserialization (PR #10)

## [1.1.3]

### Changed
- `SetActiveWorkspaceFor` is now obsolete due to removal from experimental 
- `DeleteWorkspaceAsync` is now obsolete because of removal SetActiveWorkspaceFor endpoint from API.
### Fixed
- `LongRunning` is `UserSettingsDto` is now a bool as it should be (Issue #8)


## [1.1.2]

### Fixed
- `projectRequired` and `considerDurationFormat` were mixed
- Clockify api requires ISO-8601 format for dates otherwise PM part 12-24 will be lost


## [1.1.1]

### Changed
- Change paramater name in `DeleteTimeEntryAsync` to timeEntryId
### Fixed
- DataOffset formating in `FindAllTimeEntriesForUserAsync()`

## [1.1.0]

### Added
- Support for POST /users/{userId}/activeWorkspace/{workspaceId}
### Changed
- Updated RestSharp
- Code to stopped using obselete methods.
### Removed
- Removed Q&A dependencies

## [1.0.0]

### Added
- Support for all endpoints form https://clockify.me/developers-api
	- Workspace support
	- User support
	- Client support
	- Projects support
	- Tag support
	- Task support
	- Time Entry support
	- Template support

<!-- 
===== Template =====
## [0.0.0]
### Added
### Changed
### Removed 
### Fixed
-->
