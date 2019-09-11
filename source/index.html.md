---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - shell
  - javascript

toc_footers:
  - <a href='https://sareye.com'>Our website</a>
  - <a href='https://sareye.sardynamics.com/demo_requests/new?mobile=0'>Contact us</a>

includes:
  - areas
  - checklists
  - courses
  - devices
  - dispatch_groups
  - dispatch_response_types
  - dispatch_responses
  - dispatches
  - groups
  - issue_types
  - issues
  - kinds
  - leader_types
  - leaders
  - maintenances
  - marker_types
  - operation_logs
  - operation_scales
  - operation_types
  - operation_view_history
  - operations
  - plans
  - priorities
  - resources
  - risk_templates
  - risks
  - rounds
  - surveys
  - tags
  - tasks
  - trackers
  - triage_location_types
  - triage_status_types
  - triages
  - units
  - users
  - errors

search: true
---

# Introduction

Welcome to the SAReye API! You can use our API to access SAReye API endpoints, which can get information on various items in our database.

We have language bindings in Shell, Ruby, Python, and JavaScript! You can view code examples in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right.

# Authentication

SAReye uses API keys to allow access to the API. You can register for a new API key at your user setup page http://{your_tenants_subdomain}.sardynamics.com/users

SAReye expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e`

<aside class="notice">
You must replace <code>abbe0983-7b75-53df-bc32-009b79d2c61e</code> with your personal API key.
</aside>
