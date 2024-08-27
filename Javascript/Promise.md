
[[NestJS]]
```Typescript
public async uploadCsvFile(
		@Query() params: MessageRequestParams,
		@Res() res: Response,
		@UploadedFile() file
	): Promise<string>{
		...
		resolve(JSON.stringify(email_content));
	}
```