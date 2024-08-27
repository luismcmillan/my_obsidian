[[NestJS]]
```Typescript
import {ApiProperty} from '@nestjs/swagger'
import {IsArray, IsBoolean, IsNumberString, IsOptional, IsString} from ...

export class MessageRequestParams {
	
	@ApiProperty({example: 1, description: 'blabla'})
	@IsNumberString()
	public from: number;
	
	@ApiProperty({example: 'de', description: 'blabla'})
	@IsString()
	public to: string;
}
```

``` Typescript
import { MiauService } from 'miaufile';

@Injectable()
@Controller()
@Apitags('lili')
export class LuisService {

	@Inject()
	private miau: MiauService

	@Post('getCat')
	public async uploadCsvFile(
		@Query() params: MessageRequestParams,
		@Res() res: Response,
		@UploadedFile() file
	): Promise<string>{
		try{
		}catch (err) {
			res.status(500).send({error: 'Failed'})
		}
	}


}
```

