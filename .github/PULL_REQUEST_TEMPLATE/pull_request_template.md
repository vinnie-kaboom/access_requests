name: Access Request
assignees: []

body:
  - type: input
    id: requestor_name
    attributes:
      label: Requestor Name
      description: Your full name
      placeholder: e.g. Jane Doe
    validations:
      required: true

  - type: input
    id: github_username
    attributes:
      label: GitHub Username
      description: Your GitHub username
      placeholder: e.g. janedoe
    validations:
      required: true

  - type: input
    id: email
    attributes:
      label: Email Address
      description: Your work email address
      placeholder: e.g. jane.doe@company.com
    validations:
      required: true

  - type: input
    id: resource
    attributes:
      label: Resource/Repository/Service
      description: What do you need access to?
      placeholder: e.g. repo-name, system, etc.
    validations:
      required: true

  - type: dropdown
    id: type_of_access
    attributes:
      label: Type of Access
      description: Select the type of access you need
      options:
        - Read
        - Write
        - Execute
    validations:
      required: true

  - type: textarea
    id: reason
    attributes:
      label: Reason for Access
      description: Why do you need this access?
    validations:
      required: true

  - type: input
    id: manager_github
    attributes:
      label: Manager's GitHub Username
      description: Who should approve this request?
      placeholder: e.g. @manager
    validations:
      required: true

  - type: input
    id: date_needed
    attributes:
      label: Date Needed
      description: When do you need access?
      placeholder: e.g. 2024-06-01
    validations:
      required: true

  - type: textarea
    id: additional_notes
    attributes:
      label: Additional Notes
      description: Any other relevant information

  - type: markdown
    attributes:
      value: |
        ---
        ## Approval Section (For Reviewer)

        **Decision:**  
        - [ ] Approve  
        - [ ] Reject  

        **Reason for Rejection (if rejected):**  
