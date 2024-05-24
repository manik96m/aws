## Cloud Formation

- Defining Infrastructure as code
- Makes it easier to manage multiple services
- Makes it easier to rebuild infrastructure and applications
- Users can create and manage a collections of AWS resources
- Resources can be provisioned and updated in an orderly and predictable manner

## Templates

- Format JSON/YAML
- Describes AWS infrastructure
- Cloud Formation designer or text editor can be used to create a template
- Templates can be reused to replicate infrastructure in multiple environments
- They can be made reusable by using parameters, mapping and conditions sections
- Template consists of nine main objects
  - Format Version
  - Description - Details about the template
  - Metadata
  - Parameters - Used for Customizing stack
  - Mappings
  - Conditions - optional - define when a resource is created
  - Transform - optional -
  - Resources - required - Resource to provision in stack
  - Outputs - optional - Declare resource data in console

## How Cloud Formation works?

- Code template is saved locally or in S3 bucket
- Cloud Formation creates stack based on the template provided
- Resources are provisioned based on the configuration provided in template

## Template Resource Attributes

- Creation Policy
  - Delaying resource configuration based on some signals
- Deletion Policy
  - By default, everything (resource + content) is deleted when a resource is deleted
  - Used for Preserving and backing up resources when stack is deleted
  - Using deletion policy, we can take a snapshot of the resource before deleting
- Depends On
  - Creation of a resource can be delayed or made dependent on another resource
- Metadata
  - Associate resource with structured data??
- Update Policy
  - Manage and replace the updates of instances??

## Stack

- Collection of AWS resources, managed as a single unit
- Cloud Formation template defines a stack in which resources are created, deleted or updated in a predictable way
- Stacks can also be nested

---

- -

- -

- -

- -

-
