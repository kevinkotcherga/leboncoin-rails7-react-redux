# README

 rails new app

 rails g scaffold post title:string body:text

 bundle add rack-cors

 rails db:migrate

 ------------------------------------------------------------------------------

config/initializers/cors.rb :

Rails.application.config.middleware.insert_before 0, Rack::Cors do
    allow do
        origins '*'
        resource '*', headers: :any, methods: %i[get post patch put delete]
    end
end

post_controller :

skip_before_action :verify_authenticity_token

def destroy
    @post.destroy

    respond_to do |format|
      format.html { redirect_to posts_url, notice: "Post was successfully destroyed." }
      format.json { render json: Post.all, status: :ok }
    end
  end

def post_params
      params.require(:post).permit(:title, :body, :id)
end

copy :
controller/concerns/authoriziable
lib/auth0_client.rb
config/auth0.yml
.dockerignore
.env
docker-compose.yml
dockerfile

git clone git clone https://github.com/auth0-developer-hub/spa_react_javascript_hello-world.git --branch basic-authentication

npm i sass axios react-redux redux redux-devtools-extension redux-logger redux-thunk

index.html :
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>
# leboncoin-rails7-react-redux
