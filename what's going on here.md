npm init
npm i react react-dom
npm i --save-dev @babel/core @babel/preset-env @babel/preset-react babel-loader file-loader css-loader sass-loader sass style-loader webpack webpack-cli webpack-dev-server
build
npm run serve
and this auto uploads chages to live page for dev yay

when you are done
npm run build
(THIS is when you get the dist folder btw)

# optional
NPM --save-dev mini-css-extract plugin 
in webpack.config 
const MiniCssExtractPlugin
# replace style loader with MiniCssExtractPlugin, loader, 
and at end
         'sass-loader'
                ]
            }
        ]
    },
    plugins: [new MiniCssExtractPlugin]
};
# add main.css to your html file
run build again
now your build dist folder has a main.css 