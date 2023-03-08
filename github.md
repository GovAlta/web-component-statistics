# Github API

#### Get all issues of a repo
```
gh api repos/GovAlta/ui-components/issues
```

####  Get all repos of the organization
``
gh api orgs/GovAlta/repos
``

#### Get Repo Statistic/Profile

```
gh api repos/GovAlta/ui-components/community/profile
{
  "health_percentage": 62,
  "description": "ui-components contains the code you need to start building a user interface for Government of Alberta platforms and services.",
  "documentation": null,
  "files": {
    "code_of_conduct": null,
    "code_of_conduct_file": null,
    "contributing": {
      "url": "https://api.github.com/repos/GovAlta/ui-components/contents/contributing.md",
      "html_url": "https://github.com/GovAlta/ui-components/blob/alpha/contributing.md"
    },
    "issue_template": null,
    "pull_request_template": null,
    "license": {
      "key": "apache-2.0",
      "name": "Apache License 2.0",
      "spdx_id": "Apache-2.0",
      "url": "https://api.github.com/licenses/apache-2.0",
      "node_id": "MDc6TGljZW5zZTI=",
      "html_url": "https://github.com/GovAlta/ui-components/blob/alpha/LICENSE"
    },
    "readme": {
      "url": "https://api.github.com/repos/GovAlta/ui-components/contents/README.md",
      "html_url": "https://github.com/GovAlta/ui-components/blob/alpha/README.md"
    }
  },
  "updated_at": "2021-10-22T19:52:46Z",
  "content_reports_enabled": false
}
```

#### Get Trafic
```
gh api repos/GovAlta/ui-components/traffic/clones      
{
  "count": 141,
  "uniques": 36,
  "clones": [
    {
      "timestamp": "2023-02-22T00:00:00Z",
      "count": 6,
      "uniques": 2
    },
    {
      "timestamp": "2023-02-23T00:00:00Z",
      "count": 13,
      "uniques": 5
    },
    {
      "timestamp": "2023-02-24T00:00:00Z",
      "count": 11,
      "uniques": 3
    },
    {
      "timestamp": "2023-02-25T00:00:00Z",
      "count": 1,
      "uniques": 1
    },
    {
      "timestamp": "2023-02-27T00:00:00Z",
      "count": 13,
      "uniques": 6
    },
    {
      "timestamp": "2023-02-28T00:00:00Z",
      "count": 6,
      "uniques": 1
    },
    {
      "timestamp": "2023-03-01T00:00:00Z",
      "count": 33,
      "uniques": 9
    },
    {
      "timestamp": "2023-03-02T00:00:00Z",
      "count": 10,
      "uniques": 6
    },
    {
      "timestamp": "2023-03-03T00:00:00Z",
      "count": 12,
      "uniques": 5
    },
    {
      "timestamp": "2023-03-04T00:00:00Z",
      "count": 1,
      "uniques": 1
    },
    {
      "timestamp": "2023-03-05T00:00:00Z",
      "count": 3,
      "uniques": 2
    },
    {
      "timestamp": "2023-03-06T00:00:00Z",
      "count": 6,
      "uniques": 3
    },
    {
      "timestamp": "2023-03-07T00:00:00Z",
      "count": 26,
      "uniques": 15
    }
  ]
}
```

#### Top referral
Get the top 10 referrers over the last 14 days.

```
 % gh api repos/GovAlta/ui-components/traffic/popular/referrers
[
  {
    "referrer": "github.com",
    "count": 300,
    "uniques": 24
  },
  {
    "referrer": "abgov-ui-react.netlify.app",
    "count": 14,
    "uniques": 2
  },
  {
    "referrer": "cac-powerpoint.officeapps.live.com",
    "count": 12,
    "uniques": 2
  },
  {
    "referrer": "ui-components-ui-components-dev.os99.gov.ab.ca",
    "count": 5,
    "uniques": 1
  },
  {
    "referrer": "Google",
    "count": 1,
    "uniques": 1
  }
]
```

**Views**
Get the total number of views and breakdown per day or week for the last 14 days. Timestamps are aligned to UTC midnight of the beginning of the day or week. Week begins on Monday.

```
gh api repos/GovAlta/ui-components/traffic/views            
{
  "count": 1321,
  "uniques": 48,
  "views": [
    {
      "timestamp": "2023-02-22T00:00:00Z",
      "count": 85,
      "uniques": 10
    },
    {
      "timestamp": "2023-02-23T00:00:00Z",
      "count": 112,
      "uniques": 10
    },
    {
      "timestamp": "2023-02-24T00:00:00Z",
      "count": 169,
      "uniques": 20
    },
    {
      "timestamp": "2023-02-25T00:00:00Z",
      "count": 14,
      "uniques": 2
    },
    {
      "timestamp": "2023-02-27T00:00:00Z",
      "count": 256,
      "uniques": 13
    },
    {
      "timestamp": "2023-02-28T00:00:00Z",
      "count": 123,
      "uniques": 10
    },
    {
      "timestamp": "2023-03-01T00:00:00Z",
      "count": 240,
      "uniques": 12
    },
    {
      "timestamp": "2023-03-02T00:00:00Z",
      "count": 91,
      "uniques": 8
    },
    {
      "timestamp": "2023-03-03T00:00:00Z",
      "count": 78,
      "uniques": 7
    },
    {
      "timestamp": "2023-03-06T00:00:00Z",
      "count": 73,
      "uniques": 6
    },
    {
      "timestamp": "2023-03-07T00:00:00Z",
      "count": 80,
      "uniques": 8
    }
  ]
}

```

#### Get all content 
```
gh api repos/GovAlta/ui-components/contents/
```
