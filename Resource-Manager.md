# Resource Hierarchy

Google resources are broken down into 4 layers
* Organisation (root node) - represents the company
* Folder (optional)
* Project
* Resource

Policies can be set on all layers of the hierarchy and are transative at any layer
**NOTE - Permissive parent permissions will override a more restrictive child policy**

Constraints restrict gcp services and is usually applied to the organisation and inherited by all child resources

## Super Admin best practices
Super Admin user is created when creating an organisation - **Super admin account should not be used for day to day functions**

* Use an email that is not tied to the organisation
* Enable MFA - use a physical MFA device
* Use stackdriver alerts for Super Admin useage
* Create a group for Organisation Admin using least privilege - keep super admin seperate from this group


