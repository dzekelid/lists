---
name: Twilio
x-slug: twilio
description: Cloud communications platform for building SMS, Voice & Messaging applications
  on an API built for global scale. Get started with a free trial.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
x-kinRank: "10"
x-alexaRank: "9195"
tags: Lists
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/apis.md
specificationVersion: "0.14"
apis:
- name: Twilio Delete SIP Credential From List
  x-api-slug: twilio
  description: Remove a Credential from a CredentialList.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/CredentialLists/{CLSid}/Credentials/{CredentialSid}
  tags: SIP Credential Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsidcredentialscredentialsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsidcredentialscredentialsid-delete-openapi.md
- name: Twilio Get SIP Credentials List
  x-api-slug: twilio
  description: Get a specific Credential in a list. Though a password is stored for
    each username in your list, the password is not returned to protect your password.
    If you cannot remember your password, you will need to POST to this resource to
    update it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/CredentialLists/{CLSid}/Credentials/{CredentialSid}
  tags: SIP Credential Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsidcredentialscredentialsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsidcredentialscredentialsid-get-openapi.md
- name: Twilio Add To SIP Credentials List
  x-api-slug: twilio
  description: Change the password of a Credential record.nnIf the change is successful,
    Twilio will respond with the Credential record but will not include the password
    in the response.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/CredentialLists/{CLSid}/Credentials/{CredentialSid}
  tags: SIP Credential Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsidcredentialscredentialsid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsidcredentialscredentialsid-post-openapi.md
- name: Twilio Get SIP Credentials List
  x-api-slug: twilio
  description: Get the list of Credentials in a CredentialList. The passwords for
    the Credentials are intentionally not returned so as to protect them.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/CredentialLists/{CLSid}/Credentials
  tags: SIP Credential Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsidcredentials-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsidcredentials-get-openapi.md
- name: Twilio Get SIP Credentials List
  x-api-slug: twilio
  description: Add a Credential to the CredentialList.nnWhen creating a Credential,
    you will POST both a username and password, but only receive the username back
    in the response. The password is intentionally not returned so as to protect it.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/CredentialLists/{CLSid}/Credentials
  tags: SIP Credential Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsidcredentials-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsidcredentials-post-openapi.md
- name: Twilio Delete SIP Credential List
  x-api-slug: twilio
  description: Delete a CredentialList from your account. It can only be deleted if
    no domains are mapped to it. If you attempt to delete one that is mapped to a
    domain, you will receive an error.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/CredentialLists/{CLSid}
  tags: SIP Credential Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsid-delete-openapi.md
- name: Twilio Get SIP Credentials List
  x-api-slug: twilio
  description: Get a credential list instance resource
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/CredentialLists/{CLSid}
  tags: SIP Credential Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsid-get-openapi.md
- name: Twilio Add SIP Credentials List
  x-api-slug: twilio
  description: Change the FriendlyName of the list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/CredentialLists/{CLSid}
  tags: SIP Credential Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallistsclsid-post-openapi.md
- name: Twilio Get SIP Credentials List
  x-api-slug: twilio
  description: Gets a list of Credential Lists for an account
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/CredentialLists
  tags: SIP Credential Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallists-get-openapi.md
- name: Twilio Get SIP Credentials List
  x-api-slug: twilio
  description: Create a new Credential List.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/CredentialLists
  tags: SIP Credential Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallists-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipcredentiallists-post-openapi.md
- name: Twilio Delete SIP IP Access Control List IP Address
  x-api-slug: twilio
  description: Deletes an IP address entry from the list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/IpAccessControlLists/{IpAccessControlListSid}/IpAddresses/{IpAddressSid}
  tags: SIP IP Access Control Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsidipaddressesipaddresssid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsidipaddressesipaddresssid-delete-openapi.md
- name: Twilio Get SIP IP Access Control List IP Address
  x-api-slug: twilio
  description: Return a single IP Address resource.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/IpAccessControlLists/{IpAccessControlListSid}/IpAddresses/{IpAddressSid}
  tags: SIP IP Access Control Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsidipaddressesipaddresssid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsidipaddressesipaddresssid-get-openapi.md
- name: Twilio Add SIP IP Access Control List IP Address
  x-api-slug: twilio
  description: Change the description or IP address of a given IpAddress instance
    resource
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/IpAccessControlLists/{IpAccessControlListSid}/IpAddresses/{IpAddressSid}
  tags: SIP IP Access Control Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsidipaddressesipaddresssid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsidipaddressesipaddresssid-post-openapi.md
- name: Twilio Get SIP IP Access Control List IP Address
  x-api-slug: twilio
  description: List the IP Addresses contained in this list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/IpAccessControlLists/{IpAccessControlListSid}/IpAddresses
  tags: SIP IP Access Control Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsidipaddresses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsidipaddresses-get-openapi.md
- name: Twilio Add SIP IP Access Control List IP Address
  x-api-slug: twilio
  description: Add an IP Address to the list with a description.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/IpAccessControlLists/{IpAccessControlListSid}/IpAddresses
  tags: SIP IP Access Control Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsidipaddresses-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsidipaddresses-post-openapi.md
- name: Twilio Delete SIP IP Access Control List IP Address
  x-api-slug: twilio
  description: Delete an IpAccessControlList from your account. It can only be deleted
    if no domains are mapped to it. If you attempt to delete one that is mapped to
    a domain, you will receive an error.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/IpAccessControlLists/{IpAccessControlListSid}
  tags: SIP IP Access Control Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsid-delete-openapi.md
- name: Twilio Get SIP IP Access Control List IP Address
  x-api-slug: twilio
  description: Return a specific IpAccessControlList resource.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/IpAccessControlLists/{IpAccessControlListSid}
  tags: SIP IP Access Control Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsid-get-openapi.md
- name: Twilio Add SIP IP Access Control List IP Address
  x-api-slug: twilio
  description: Rename an IpAccessControlList.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/IpAccessControlLists/{IpAccessControlListSid}
  tags: SIP IP Access Control Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsid-post-openapi.md
- name: Twilio Get SIP IP Access Control List
  x-api-slug: twilio
  description: Return a paged list of all IpAccessControlLists under this account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/IpAccessControlLists
  tags: SIP IP Access Control Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollists-get-openapi.md
- name: Twilio Add SIP IP Access Control List
  x-api-slug: twilio
  description: Create a new IpAccessControlList resource.nnWhen created, the list
    will contain no IP addresses. You will need to add IP addresses to the list for
    it to be active. To add IP addresses, you will need to POST to the IpAddresses
    List subresource.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01///Accounts/{AccountSid}/SIP/IpAccessControlLists
  tags: SIP IP Access Control Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollists-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/accountsaccountsidsipipaccesscontrollists-post-openapi.md
- name: Twilio
  x-api-slug: twilio
  description: Cloud communications platform for building SMS, Voice & Messaging applications
    on an API built for global scale. Get started with a free trial.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01/
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twilio/openapi.md
x-common:
- type: x--net-library
  url: https://www.twilio.com/docs/csharp/install
- type: x-acceptable-use-policy
  url: https://www.twilio.com/legal/aup
- type: x-application-gallery
  url: https://www.twilio.com/showcase
- type: x-base-url
  url: https://api.twilio.com
- type: x-blog
  url: http://www.twilio.com/blog
- type: x-blog-rss
  url: http://www.twilio.com/blog/feed
- type: x-community-supported-libraries
  url: https://www.twilio.com/docs/libraries
- type: x-contact-form
  url: https://www.twilio.com/help/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/twilio
- type: x-crunchbase
  url: https://crunchbase.com/organization/twilio
- type: x-documentation
  url: https://www.twilio.com/docs/api
- type: x-email
  url: help@twilio.com
- type: x-email
  url: privacy@twilio.com
- type: x-email
  url: legalnotices@twilio.com
- type: x-email
  url: trademark@twilio.com
- type: x-email
  url: kyleky@twilio.com
- type: x-getting-started
  url: https://www.twilio.com/docs/quickstart
- type: x-github
  url: https://github.com/twilio
- type: x-how-to-guides
  url: https://www.twilio.com/docs/howto
- type: x-java-library
  url: https://www.twilio.com/docs/java/install
- type: x-node-js-library
  url: https://www.twilio.com/docs/node/install
- type: x-paid-support
  url: https://www.twilio.com/premium-support#features
- type: x-partners
  url: https://www.twilio.com/partners
- type: x-php-library
  url: https://www.twilio.com/docs/php/install
- type: x-pricing
  url: https://www.twilio.com/pricing
- type: x-privacy
  url: https://www.twilio.com/legal/privacy
- type: x-python-library
  url: https://www.twilio.com/docs/python/install
- type: x-ruby-library
  url: https://www.twilio.com/docs/ruby/install
- type: x-salesforce-pdk
  url: https://www.twilio.com/docs/salesforce/install
- type: x-security
  url: https://www.twilio.com/docs/security
- type: x-service-level-agreement
  url: https://www.twilio.com/legal/service-level-agreement
- type: x-stack-overflow
  url: http://stackoverflow.com/questions/tagged/twilio
- type: x-status
  url: http://status.twilio.com/
- type: x-status-rss
  url: http://status.twilio.com/rss
- type: x-terms-of-service
  url: https://www.twilio.com/legal/tos
- type: x-trademarks
  url: https://www.twilio.com/legal/trademark
- type: x-transparency-report
  url: https://www.twilio.com/blog/2015/07/transparency-report-for-government-requests-for-customer-information.html
- type: x-transparency-report
  url: https://www.twilio.com/legal/transparency
- type: x-twitter
  url: https://twitter.com/twilio
- type: x-website
  url: http://www.twilio.com
- type: x-website
  url: http://twilio.com
- type: x-website
  url: http://stackoverflow.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---