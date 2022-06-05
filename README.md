# VODManagement
Requirements

Content and license models must be defined.


Content

o id

o name

o status

o licenses (ManyToMany)

o videoUrl

License

o id

o name

o startTime

o endTime

o contents (ManyToMany)

-Crud apis and management uis required for content and license.

-Content status field can be two different value. (InProgress, Published)

-VideoUrl is a text field. It will be editable on ui.

-Multiple licenses can be attached to content. But these licenses time windows can not be overlaped.

-When content created first time, content status will be in progress.VideoUrl and at least one license required to content to pass Published status.

-Content status will be published automatically when content is in its any license time window. Also content status will return InProgress automatically when content’s
license time has ended.
