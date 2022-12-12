Backing up the server

To back up the server I'd consider two approaches depending on available tooling
Cloud Agnostic

For a cloud agnostic approach, I'd consider using a tool like rsync to back up files to a remote host. This could be done using the 3-2-1 strategy with the backup stored in three different places in at least two different physical locations.

I'd consider a scheme such as daily, weekly, and monthly backups.
AWS

For AWS server instances, I'd use the AWS Backup service with a sensible policy defining the frequency and retention policy.

For data renention, we'd likely be limited or guided by regulatory requirements.